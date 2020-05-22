Updated: {docsify-updated}

# Tasker Support

Texpand allows you to use Tasker built-in and user created variables in your phrases, additionally you can trigger Tasker actions by typing a shortcut. 

In this page you will learn how to use Texpand's Tasker integration.

> <i class='bx bxs-crown' style="color: orange"></i> Tasker integration is part of Texpand premium.

## Using Tasker built-in variables

Tasker opens up a wide range of of  global built in
<a href="https://tasker.joaoapps.com/userguide/en/variables.html" target="_blank">variables</a>, you can use these variables in your phrases. Before you can use Takser built-in variables in your phrases you need configure Texpand plugin with Tasker, here's how:

1. Open Tasker and tap the '+' button to create a profile, then navigate to: *Event → Plugin -> Texpand → Request Tasker built-in variables update*

2. This will open a new screen titled "Event Edit" while in this screen tap the pencil button on the right side of "Configuration" label, then a plugin configuration screen will be come up then tap the switch to turn the plugin on, finally press the back button twice.

3. Tap "New Task +", Tasker will ask you to name it, give it a name to proceed.

4. This will open "Task Edit" screen, tap the '+' button on the bottom right, then navigate to: *Plugin → Texpand → Update built-in Tasker variables*

5. A new screen titled "Action Edit" will be opened, then tap the pencil button to the right of the "Configuration" label, in the screen that comes up, tap the switch to turn the action plugin on and go back to Tasker's profiles screen.

6. That's it, now you are ready to use Tasker built in variables in your phrases.

### Adding Tasker built-in variables to your phrases

1. Open Texpand and tap the '+' button then select either "Phrase" or "Phrase list"

2. Now move the cursor to either "phrase" or to "List item" in case of phrase lists, then the variable menu will appear above your keyboard.

3. Scroll horizontally to the right end of the variable menu until you see 'Tasker', once you see it tap 'Tasker' and select 'Built-in' then a dialog listing all Tasker built-in variables will be shown from here select the variable you want use, repeat this step to add more variables.

> To use your phrases with Tasker variables simply type the shortcut in a compatible application and the Tasker variables in the phrase should be replaced with thier respective values provided by Tasker.

## Tasker configuration for user variables

Texpand has support for Tasker's user created local variables. To demonstrate how to use user created local Tasker variables with Texpand, here's an example that will allow you to fetch the current Bitcoin price and use it in Texpand. You can also import this task <a href="https://taskernet.com/shares/?user=AS35m8kVZzyXnsJmz1SfMBXr%2BwhJbIG%2F%2Ff26SUe5pP3rZ3j7ECdpC1YJzSpBGW%2F8OKFd4Ll42qUApRki%2BnFiue7iUQ%3D%3D&id=Profile%3AUpdate+Bitcoin+Price+Every+15+Minutes" target="_blank">from here</a>:


1. Open Tasker and tap the '+' button to create a profile and select "Time".

2. Tap "From" and "Until" to disable them, then select "Every" and type 15 in the text field besides after that change the time unit to "Minute(s)", this will make the task run every 15 minutes.

3. Select "New Task +" and give the task a name to proceed.

4. Tap the '+' button on the bottom right, then navigate to: *Plugin → Http Request*, this will open a screen titled "Action Edit".

5. Scroll down and you will find a text field titled "URL" then enter "https://blockchain.info/ticker" which is a site that provides bitcoin exchange rate data. Go back once you have entered the url.

6. Tap the '+' button on the bottom right, then navigate to: *Variables → Variable Set*

7. In the text field titled "Name" enter 'btc_exch_rate' below there's another text field titled "To" simply enter a space here and go back.

8. Tap the '+' button on the bottom right, then navigate to: *Code → Javascriptlet Set*

9. Under the text field titled "Code" enter the following javascript code `btc_exch_rate = JSON.parse(http_data).USD.last` and go back

10. Tap the '+' button on the bottom right and navigate to: *Plugin → Update Tasker user variables*

11. Tap the pencil button besides "Configuration" then a screen listing available variables will open here check 'btc_exch_rate', this step will send the updated value of the variable 'btc_exch_rate' to Texpand when this task runs.

### Using local user created variables to your phrases

1. Open Texpand and tap the '+' button then select either "Phrase" or "Phrase list"

2. Now move the cursor to either "phrase" or to "List item" in case of phrase lists, then the variable chooser toolbar will appear above your keyboard.

3. Scroll to the right end of the variable chooser toolbar until you see 'Tasker', once you see it tap it and select 'User vars' then a dialog listing available  variables will be shown from here select the variable you want use, repeat this step to add more variables. As per the above example 'btc_exch_rate' should show up here, if you select it Texpand will replace it with Bitcoin current exchange rate when expand it using it's respective shortcut.