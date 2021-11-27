# Amplify and Cognito


The Amplify Framework uses Amazon Cognito as the main authentication provider. Amazon Cognito is a robust user directory
service that handles user registration, authentication, account recovery & other operations.

![cognito](https://www.google.com/url?sa=i&url=https%3A%2F%2Faws.amazon.com%2Far%2Fgetting-started%2Fhands-on%2Fbuild-serverless-web-app-lambda-apigateway-s3-dynamodb-cognito%2F&psig=AOvVaw2x8TBSWWc_D4TPkceQEvpC&ust=1638125919418000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCKDUvOGcufQCFQAAAAAdAAAAABAJ)

![cognito](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2Fanalytics-vidhya%2Fwhat-is-aws-amplify-advantages-and-disadvantages-of-aws-amplify-49ddc4831467&psig=AOvVaw2x8TBSWWc_D4TPkceQEvpC&ust=1638125919418000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCKDUvOGcufQCFQAAAAAdAAAAABAg)



### dependencies for cognito

```
dependencies {
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
}
```

### Initialize Amplify Auth

```
// Add this line, to include the Auth plugin.
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.configure(getApplicationContext());
```
