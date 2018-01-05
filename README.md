# Recyclerview-with-Gridview
Android GridLayoutManager is the RecyclerView.LayoutManager implementation to lay out items in a grid. In this tutorial, we’ll create an application that displays CardViews inside a RecyclerView in the form of a GridLayout.

Also, we’ll implement an interface that makes RecyclerView item click similar to a ListView itemClickListener.

<h4>Android GridLayoutManager</h4>
We’ve implemented a RecyclerView using a LinearLayoutManager here. Now let’s use a GridLayoutManager to layout the RecyclerView as a grid.

Following is the constructor for a GridLayoutManager.
```
GridLayoutManager (Context context, 
                int spanCount, 
                int orientation, 
                boolean reverseLayout)
```

everseLayout if set true then layout items from end to start.

To set the span size for each item, we invoke the method setSpanSizeLookup on the GridLayoutManager

1. The above class implements the interface RecyclerViewAdapter.ItemListener and overrides the method onItemClick that’s defined in the adapter class. By doing this, we’ve implemented the RecyclerView Click Listener within our Activity instead of the Adapter class(similar to the standard onItemClickListener defined for a ListView)
2. A DataModel class holds the details for each RecyclerView item
3. The LayoutManager of the RecyclerView can be defined by either instantiating the AutoFitGridLayoutManager class with the column width set as 500 or by invoking the GridLayoutManager class object and setting the number of columns as 2
<br></br>
<a href="url"><img src="https://github.com/sambhaji213/Recyclerview-with-Gridview/blob/master/screenshot/device.png" align="left" height="480" width="300"></a>


