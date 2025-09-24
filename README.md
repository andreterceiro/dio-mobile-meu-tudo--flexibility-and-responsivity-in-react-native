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