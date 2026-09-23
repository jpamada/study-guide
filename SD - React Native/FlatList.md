#### Definition

**FlatList**
Allows to render items efficiently.

___
#### Props

**[[data]]**
The array of data that FlatList renders. This props is required.

**[[renderItem]]**
A function that receives each item from data and returns the React element that should be rendered. This prop is required. 

**[[keyExtractor]]**
Specifies the key for each item.

**[[ListEmptyComponent]]**
Component displayed when data contains no items.

**[[ListHeaderComponent]]**
Renders content above the list items.

**[[ListFooterComponent]]**
Renders content after the list items.

**[[ItemSeparatorComponent]]**
Renders a component only between each item.

**[[showsVerticalScrollIndicator]]**
Controls whether the vertical scroll indicator is displayed.

**[[showsHorizontalScrollIndicator]]**
Shows/hides horizontal scrollbar.

**[[contentContainerStyle]]**
Styles the scrollable content container.

**[[horizontal]]**
Changes the list from vertical scrolling to horizontal scrolling.

**[[numColumns]]**
Specifies how many columns the list should display.

**[[onRefresh]]**
Enables pull-to-refresh behavior.

**[[refreshing]]**
Controls whether the pull-to-refresh indicator is currently visible.

**[[onEndReached]]**
Called when the list scrolls close enough to its end. Common in pagination or infinite scroll.

**[[onEndReachedThreshold]]**
Controls how close to the end the user must scroll before onEndReached fires.