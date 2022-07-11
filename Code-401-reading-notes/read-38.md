## Read 38

-  you want to return a result to the activity that invoked yours, simply call setResult() to specify the result code and result Intent. When your operation is done and the user should return to the original activity, call finish() to close (and destroy) your activity

- You must always specify a result code with the result. Generally, it's either RESULT_OK or RESULT_CANCELED. You can then provide additional data with an Intent, as necessary.

- If you simply need to return an integer that indicates one of several result options, you can set the result code to any value higher than 0. If you use the result code to deliver an integer and you have no need to include the Intent, you can call setResult() and pass only a result code.

- Explicit intents specify which application will satisfy the intent, by supplying either the target app's package name or a fully-qualified component class name. You'll typically use an explicit intent to start a component in your own app, because you know the class name of the activity or service you want to start. For example, you might start a new activity within your app in response to a user action, or start a service to download a file in the background.

- Implicit intents do not name a specific component, but instead declare a general action to perform, which allows a component from another app to handle it. For example, if you want to show the user a location on a map, you can use an implicit intent to request that another capable app show a specified location on a map.

- A PendingIntent object is a wrapper around an Intent object. The primary purpose of a PendingIntent is to grant permission to a foreign application to use the contained Intent as if it were executed from your app's own process.

-  most cases, your app should create immutable PendingIntent objects, as shown in the following code snippet. If a PendingIntent object is immutable, then other apps cannot modify the intent to adjust the result of invoking the intent.

