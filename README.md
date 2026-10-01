# DTD-Practice

## DTD

<?xml version="1.0" encoding="UTF-8"?>

<!ELEMENT recipe (recipeType,list,action+)>
<!ELEMENT recipeType (#PCDATA)>
<!ELEMENT list (ingredient+)>
<!ELEMENT ingredient (#PCDATA)>
<!ELEMENT action (#PCDATA)>


## XML

<?xml version="1.0" encoding="UTF-8"?>
<?xml-stylesheet type="text/css" href="recipe.css"?>
<!DOCTYPE recipe "Recipe.dtd">

<recipe>
  <recipeType> Cream Cheese Frosting </recipeType> 
    <list> 
      <ingredient> 8 oz cream cheese, softened </ingredient>
      <ingredient> 1 stick unsalted butter, softened </ingredient>
      <ingredient> 1 tsp vanilla extract </ingredient>
      <ingredient> 3 cups confectioners’ sugar </ingredient>
  </list>
      <action> Beat together cream cheese, butter, and vanilla until slightly fluffy </action>
      <action> Slowly add confectioners’ sugar, beating until smooth to your liking. </action>
      <action> Frost your cake, cupcake, or muffin. </action>
</recipe>


## CSS

recipe {
    background-color: #FFFFFF;
    font-family: sans-serif;
    font-size: 14px;
    text-align: left;
    width: 300px;
    height: 300px;
    display: block;
}

recipeType {
    display: block;
}

action {
    display: block;
    color: white;
}

list {
    font-size: 16px;
    color: white;
}
