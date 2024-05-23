#Connecting Maui App with LocalHost
You can seamlessly connect your Maui app with a local server by following these four simple steps:

Run Your Web API Project: Start your web API project with the HTTP protocol enabled. Take note of the port number specified in the launch configuration file.

Update Request URLs: When making requests to your local server, avoid using "http://localhost:{port}". Instead, utilize "http://10.0.0.2:{port}" as the base URL.

Configure Android Application: Navigate to Platforms\Android\MainApplication.cs and replace [Application] with [Application(UsesCleartextTraffic = true)] to ensure proper communication with your local server.

Check Internet Permission: Confirm that the necessary internet permission is declared in the AndroidManifest folder.

By following these steps, you can seamlessly connect your emulator with your local API, facilitating smooth development and testing processes.
