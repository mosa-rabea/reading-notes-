# Amplify and Cognito


The Amplify Framework uses Amazon Cognito as the main authentication provider. Amazon Cognito is a robust user directory
service that handles user registration, authentication, account recovery & other operations.

![cognito1](https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2020/09/03/Role-based-control-Amazon-Cognito-Figure-1.png)

![cognito](https://miro.medium.com/max/1400/1*3P460MUPl6_lUEcVXfFg4Q.png)



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
