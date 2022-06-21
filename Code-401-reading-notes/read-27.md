## Read 27

### Android Shared Preference

- getSharedPreferences() — Use this if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any Context in your app.

- getPreferences() — Use this from an Activity if you need to use only one shared preference file for the activity. Because this retrieves a default shared preference file that belongs to the activity, you don't need to supply a name.

- To write to a shared preferences file, create a SharedPreferences.Editor by calling edit() on your SharedPreferences.

- Pass the keys and values you want to write with methods such as putInt() and putString(). Then call apply() or commit() to save the changes.

### Espresso Testing

- Use Espresso to write concise, beautiful, and reliable Android UI tests

- The core API is small, predictable, and easy to learn and yet remains open for customization. Espresso tests state expectations, interactions, and assertions clearly without the distraction of boilerplate content, custom infrastructure, or messy implementation details getting in the way.

- Espresso tests run optimally fast! It lets you leave your waits, syncs, sleeps, and polls behind while it manipulates and asserts on the application UI when it is at rest.

### Espresso Test Recorder

- The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code. By recording a test scenario, you can record your interactions with a device and add assertions to verify UI elements in particular snapshots of your app. Espresso Test Recorder then takes the saved recording and automatically generates a corresponding UI test that you can run to test your app.

- The Espresso API encourages you to create concise and reliable UI tests based on user actions

- Espresso tests consist of two primary components: UI interactions and assertions on View elements. UI interactions include tap and type actions that a person may use to interact with your app. Assertions verify the existence or contents of visual elements on the screen

### Tasks and the back Stack

- A task is a collection of activities that users interact with when trying to do something in your app

- The device Home screen is the starting place for most tasks. When a user touches the icon for an app or shortcut in the app launcher (or on the Home screen), that app's task comes to the foreground.

- When the current activity starts another, the new activity is pushed on the top of the stack and takes focus. The previous activity remains in the stack, but is stopped. When an activity stops, the system retains the current state of its user interface.

- A task is a cohesive unit that can move to the background when a user begins a new task or goes to the Home screen. While in the background, all the activities in the task are stopped, but the back stack for the task remains intact—the task has simply lost focus while another task takes place,

