# Read: 36 - Cognito

##### What is amplify authentication?
The amplify-authenticator component offers a simple way to add authentication flows into your app.

##### Configure Auth Category
* execute the command:
```amplify add auth```

* Enter the following when prompted:
```
? Do you want to use the default authentication and security configuration?
    `Default configuration`
? How do you want users to be able to sign in?
    `Username`
? Do you want to configure advanced settings?
    `No, I am done.
    
 ```

* push your changes to the cloud, execute the command:
```
amplify push
```



##### Install Amplify Libraries
```
dependencies {
    implementation 'com.amplifyframework:aws-auth-cognito:1.17.4'
}
```

##### Initialize Amplify Auth
Add the Auth plugin before calling Amplify.configureInitialize Amplify Auth
```
// Add this line, to include the Auth plugin.
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.configure(getApplicationContext());
```

##### Check the current auth session
 from your MainActivity’s onCreate method:
 ```
 Amplify.Auth.fetchAuthSession(
    result -> Log.i("AmplifyQuickstart", result.toString()),
    error -> Log.e("AmplifyQuickstart", error.toString())
);
```
