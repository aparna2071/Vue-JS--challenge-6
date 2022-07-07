# Vue-JS--challenge-6

## Class & style binding:
-	For eg: if we now need that if the background color green is hovered, then green socks appear & if blue background color is hovered, blue socks appear, so for that we use style binding
:style="{ backgroundColor: variant.variantColor }"
             @mouseover="updateProduct(variant.variantImage
-	Now we want that add to cart button should be disabled if product is not in stock & we have a class for disabled button in our css file that will show the button in white color if it’s disabled. So, here we need to do class binding.
<button v-on:click="addToCart" 
          :disabled="!inStock"
          :class="{ disabledButton: !inStock }"
          >
        Add to cart
        </button>
-	disabledButton class exists in css file
-	You can also bind an entire class object or array of classes to an element
- Challenge: When inStock is false, bind a class to the “Out of Stock” p tag that adds text-decoration: line-through to that element.
- Solution: Give the value of inStock in Js file, style text-decoration:line-through in CSS file & bind that css class in html file. 
- https://codepen.io/aparnasoneja/pen/abYOExo
