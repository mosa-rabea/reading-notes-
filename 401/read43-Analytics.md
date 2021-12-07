# Analytics

### Install Amplify Libraries

add these dependencies :

```
dependencies {
    // Add these lines in `dependencies`
    implementation 'com.amplifyframework:aws-analytics-pinpoint:1.24.0'
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
}
```

### Initialize Amplify Analytics

To initialize the Amplify Auth and Analytics categories you call Amplify.addPlugin() method for each category.

paste this code to your onCreate function

```
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.addPlugin(new AWSPinpointAnalyticsPlugin(this));
```

