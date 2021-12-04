# Intent Filters

![Filters](https://tutorial.eyehunts.com/wp-content/uploads/2018/06/what-is-android-Intent-Filters-examples.png)

An intent filter is an expression in an app's manifest file that specifies the type of intents that 

the component would like to receive. For instance, by declaring an intent filter for an activity, 

you make it possible for other apps to directly start your activity with a certain kind of intent.

### Add an Intent Filter

The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:

* Action: string naming the action to perform. Usually one of the platform-defined values such as ACTION_SEND or ACTION_VIEW.

* Data: description of the data associated with the intent.

* Category: Provides an additional way to characterize the activity handling the intent, usually related to the user gesture or location from which it's started.


* Each incoming intent specifies only one action and one data type, but it's OK to declare multiple instances of the \<action>, \<category>, and \<data> elements in each \<intent-filter> .




