# Introduction

Teacher said that in web we have organization in flexbox model and organization in grid layout model (as used by Bootstrap).

Teacher also said that flexfox is default and you have no aditional declarations in your code to use flexbox.


# Container and children

Teacher said that we have to keep in mind that we have a container element (father) and a children element (son).

Is simple to understand, see this code:

```
<View>
    <Text></Text>
    <View>
        <Text></Text>
        <Text></Text>
    </View>
</View>
```

The outer <View /> component has 2 childrens, a <Text /> and another <View>. The inner <View> has 2 <Text /> components as children and is children of the outer <View />. And you can apply the same idea for the other components.


# Simple example with two boxes

Please see this simple example. In this example teacher draw 2 boxes in the screen, one red and another blue. These boxes were aligned vertically.

See that the boxes was drawn with <View /> components. Please remember the basic structure. We have to define a function first (one of each box). Part of the code of this example, defining one ot the two functions:

![example with two boxes](images/example-with-two-boxes.png)

After, you have to use the component created with the function:

![using the components created with the functions](images/using-the-components-created-with-the-functions.png)

And as in this example we use <View /> inside of the function, please remember to import the <View /> component.

```
import {View} from 'react-native';   
```

Result in emulator:

![result in emulator](images/result-in-emulator.png)


# Flex

As you know and you could see in the previous example, you need to encapsulate the inner boxes in an outer box. You need to have only a father component in the application.

And if you remove "flex: 1" from the style configuration of the container?

![removing flex: 1 of the container](images/removing-flex-1-of-the-container.png)

Note: as you could see, the external container have a purple border **in this test** (not early).

And you can also insert "flex: 1" in one of the boxes:

![inserting flex: 1 in one of the boxes](images/inserting-flex-1-in-one-of-the-boxes.png)

Explanation: the red box will get all vertical area not occupied by the blue box.

The same concept is valid if you increase the height of the blue box:

![increasing the height of the blue box](images/increasing-the-height-of-the-blue-box.png)

And if you add "flex: 1" to the style configuration of the blue blox?

![flex: 1 in the blue box](images/flex-1-in-the-blue-box.png)

And to blue box as example fill all the horizontal area, please change the width configuration in style confuguration, see:

![width 100% in blue box](images/blue-box-width-100-pct.png)

As you could see, when teacher did not specify the unit (like "%") it was similar to pixels (px).