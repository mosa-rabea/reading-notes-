# Espresso

* Espresso is an open source android user interface (UI) testing framework developed by Google.
The term Espresso is of Italian origin, meaning Coffee.
Espresso is a simple,efficient and flexible testing framework.


* we use Espresso to write android tests,
* Example of Espresso test:

```
@Test
public void greeterSaysHello() {
    onView(withId(R.id.name_field)).perform(typeText("Steve"));
    onView(withId(R.id.greet_button)).perform(click());
    onView(withText("Hello Steve!")).check(matches(isDisplayed()));
}
```


### Packages

* espresso-core - Contains core and basic View matchers, actions, and assertions. See Basics and Recipes.
* espresso-contrib - External contributions that contain DatePicker, RecyclerView and Drawer actions, accessibility checks, and CountingIdlingResource.
* espresso-intents - Extension to validate and stub intents for hermetic testing.
* espresso-remote - Location of Espresso's multi-process functionality.
* espresso-web - Contains resources for WebView support.
* espresso-idling-resource - Espresso's mechanism for synchronization with background jobs.


### Create UI tests with Espresso Test Recorder

The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code.
By recording a test scenario, you can record your interactions with a device 
and add assertions to verify UI elements in particular snapshots of your app.

* Espresso Test Recorder then takes the saved recording and automatically
 generates a corresponding UI test that you can run to test your app.

* important thing to know is that Before using Espresso Test Recorder,
 make sure you turn off animations on your test device to prevent unexpected results.

* Espresso Test Recorder writes tests based on the Espresso Testing framework, 
an API in AndroidX Test. The Espresso API encourages you to create concise and reliable UI tests based on user actions.
By stating expectations, interactions, and assertions without directly accessing the underlying app’s activities and views,
this structure prevents test flakiness and optimizes test run speed.

