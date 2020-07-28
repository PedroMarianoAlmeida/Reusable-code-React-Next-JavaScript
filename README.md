# Reusable code in React, Next and JavaScript

My reusable components in React and Next.js and functions in JavaScript

## translate function
Use google cloud to translate text

### Steps:

1. Copy the translate function on the repo and insert in your project

1. Follow [this tutorial on youtube](https://www.youtube.com/watch?v=5hTlSGD4_zk&t=4s) to create an API Key (is required a credit card, but the first $300 we get credit form google, and the price for translation is $20 per million characters - check if price changes [here](https://cloud.google.com/translate/pricing))... so is quite enough to play around

1. Create an ```.env.local``` file on your project and insert your key value in a variable called ```GOOGLE_CLOUD_TRANSLATE``` (you can insert your key value on ```API_KEY``` value inside translate function, but this is risky (to others know your key and use, and you have to pay to google... so please don't do that :smile:) - And in production you will need to set as a Enviorement Variable.

1. Now you can just use the translate function (reminder: it is an async function). The first argument is the value to translate, the second is the original language and the third is the languange that you want to translate.

## React Component - Image on one side and text in another (you choose the side)

- Considerations
  - Component created using [Reactstrap](https://reactstrap.github.io/) tools
  - On screens shorter than md, the image stays always on top and text above
  
  ### Steps
  
  1. Copy Magazine.js file and past in your components folder.
  1. Insert the referene to image in ```imageAdress``` prop
  1. Insert the text in ```text``` prop
  1. Chose the side of TEXT on ```textLocation``` prop (and the image will stay on the other side)
