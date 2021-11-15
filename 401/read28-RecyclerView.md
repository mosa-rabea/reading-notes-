# dynamic lists with RecyclerView

RecyclerView library is used to dynamically create elements when we supply the data and define how each item looks.

### Key classes
the key classes are several different class which works together to build a dynamic list.

* RecyclerView is the ViewGroup that contains the views corresponding to your data.
* Each individual element in the list is defined by a view holder object.

* You define the view holder by extending RecyclerView.ViewHolder.
* The RecyclerView binds the views to their data, by calling methods in the adapter.
* You define the adapter by extending RecyclerView.Adapter.

* The layout manager arranges the individual elements in your list.
* Layout managers are all based on the library's LayoutManager abstract class.

### implementing your RecyclerView

* decide what the list or grid is going to look like.
* Design how each element in the list is going to look and behave, and extend the ViewHolder class.
* Define the Adapter that associates your data with the ViewHolder views.



### When defining the adapter, we need to override three key methods:

* onCreateViewHolder(): RecyclerView calls this method whenever it needs to create a new ViewHolder.
* onBindViewHolder(): RecyclerView calls this method to associate a ViewHolder with data.
* getItemCount(): RecyclerView calls this method to get the size of the data set.

