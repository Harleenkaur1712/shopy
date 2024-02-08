## MakueniStore AI/ML ECommerce 

Overview
inject Batch AI, Real time AI, and Generative AI into an ecommerce application.

- Custom Product Recommendations

- Instant Lost Item Cart Updates
- Interactive Chat and Vector Search for Private Enterprise Data

The MakueniStore illustrates how working with MongoDB and Google AI can create a meaningful, custom user experience and accelerate development and time to value for Square the business.

Video Walk-through of demo:

<https://drive.google.com/file/d/1dwtrRbHRW4_WLiXvs-PY1uIh_NHlakM-/view?usp=drive_link>

This document is composed of the following parts.

- [Feature Examples Walk-through]

  - [Analytics]
  - [Batch AI for Product Recommendation Predictions]
  - [Real time AI for Lost Item Cart Updates]
  - [Generative AI for interactive chat and product suggestions based on private data]
  - [How to Recreate on Your Own Atlas Cluster]
  - [How to Customize]
  - [Change the User and Product Recommendations]
  - [Change the Chat Content ]

## Resources & Links

Link to live application (same link - bit.ly easier to remember):

<https://makuenistore.netlify.app/>



Video Walk-through of demo:


API to allow the customer to interact in a very natural way with MakueniStore, asking for advice. MakueniStore responds by generating new content (hence “generative” AI) in the form of advice. It also searches MakueniStore’s private data, whether in the product collection, previous reviews from other customers, Q&A, etc, to offer even more specific product suggestions.

## How we built it

#### Step 1. Prepared Data in MongoDB Atlas running on google cloud
Stood up an Atlas cluster. Created a database named “makueniStore” with 2 collections “products” and “customers” with the .json files in the git repository.
#### Step 2. Created Search Index named “default” on products collection 
The default dynamically mapped index will work but this one is more specific. Make sure to name the index “**default**”.
#### Step 3. 
Integrating Square APIs (Orders API, Catalog API, and Inventory API) into MakueniStore using React .
We get a list of catalog objects and once we receive data from the Square APIs, we can parse and display it in our React components. For example, we use the data to populate product listings, order history, or inventory status.

#### Step 4. 
Integrated  generative AI capabilities and the PaLM API into our React , then built a powerful conversational AI chatbot using Google's PaLM API 2, set up the PaLM account, integrate the API, and create an engaging chatbot interface
## Challenges we ran into
We delayed getting our API key , at first we had to hard-coded in the front end. We had to create a component , then build a message Exchange array. 
## Accomplishments that we're proud of
We built a strong connections and positive working relationships with the teammates that we hope wil continue in the future projects.
## What we learned
Learn how to set up the PaLM account, integrate the API, and create an engaging chatbot interface
## What's next for Makueni store
Provide documentation for Square sellers on how to use our pruduct with the integrated Square APIs and  offer customer support to address any questions or issues related to the integration.


## Features

MakueniStore, an online retailer,  captures customer’s activity, such as clicks, views, purchases, etc. The application  then applys training models, both batch and in real-time, to make product recommendations custom for this user. If items in the customer’s cart go out of stock, MakueniStore can immediately recommend similar products, thus reducing friction for the user.

Finally, MakueniStore integrates a powerful conversational AI chatbot using Google's PaLM API 2 to create an engaging chatbot  to allow the customer to interact in a very natural way with MakueniStore, asking for advice. MakueniStore responds by generating new content (hence “generative” AI) in the form of advice. It also searches MakueniStore’s private data, whether in the product collection, previous reviews from other customers, Q&A, etc, to offer even more specific product suggestions.

### Feature 1: Batch Predictive AI - Product Recommendations

Login and compare 2 different user’s product recommendations:

![](https://lh3.googleusercontent.com/r_xXDCDG775_XdQj0aqa07LEw9wl0aezYEAZfHeTCRMRzbfUiLTL9S09OHXXllZ2rJo7fxP8tJGuRVRu8IW2Z8LHAc2qMPO52gMXCZkFSCaszzjt6_PfJaCDQbqrLSAZw_vw42SuFZRwbWt2v4VIiTI)

|                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------- |
**User Profile 1:** - (This user would be a good one to change as a speaker, ex. “Logging into my account - and modify the code as per instructions below)

[karen@gmail.com](mailto:karen@gmail.com) (MUST)

Password: &lt;type anything - just hit enter >

![](https://lh4.googleusercontent.com/JmpFPE-K0rvBRNt26PYdTgQ8ehXW5uAi5jH7apc9cxG2SyN_lgw_OM3_zi1gMN0Y-NqtEXCJ49FubtE20W-VzrqbdCXeZz2asjzQKqA5YP6DOgIZdQ8izfTu-M0RhUXacMvCmc4nDVLKO7oRWjVH92U)

**User Profile 2: Our buddy Scott on his first camping trip**

[scott@streammeup.com](mailto:scott@streammeup.com)

Password: &lt;type anything - just hit enter >

![](https://lh6.googleusercontent.com/wbShTOyAZbH2Rlp5jxCYN_148VddwhJxUJxJSEL3LD_OkGXWMbO3SAanW33T7LncR7m9BQzZN8m1FLs5G6glpvoqjNdUJ4kXGiJabN4gf6xwOAAvXjpxJ0Hd3FHIAmYehyJUgNjFuISsFVjh3ZhhcNU)

## Feature 2: Traditional Analytics - Customer Behavior Activity

Click on the user profile and simple 1 sentence : Because we have been capturing data about the user’s interactions with the application…. And close.

Can use for either User 1 or User 2

![](https://lh6.googleusercontent.com/VLwbn4O711w-oxi-GcmibLvo5_95hRdfaX9Dn-3kl6I9vWRIrFu3y8Ewy1s5xS0D3iWN_N3rUoPL_-XqjTBZ8tLO1y_NsCvPiha4JU9jYRD__ZF_XpkHPRPACUZrzTrRR9sM_XhoD3PeA0JeayZMR10)

## Feature 3: Real-time AI - Lost Item in Cart Update

**Step 1:**
Once logged into Scott’s account, show the items he has in his shopping cart:- Tent - Hiking shoes - headlamp |

<img src="https://lh6.googleusercontent.com/wkq_SWI3fza_NDsNB_Wjjo5yk28XF0n2MDujqEX0EPAEkgGPoVFZhV1Thu0TAvZeDsXhO4ytibSd-lhmbeq980DQsRkHxl853PHPNYyuAQO_TX1WZmUltkQ-m_lnHUxSbaILj9d4kQKyzi7JwFGDozw" alt="drawing" width="260"/>

**Step 2:**
3 seconds afterwards (no user interaction necessary), the headlamp will go out of stock and Scott will be prompted with similar items as replacements.Generated by live click data about these products from all users being streamed into a real time engine…

<img src="https://lh6.googleusercontent.com/ElLh9WvMyzgku_18AYD3w5ujy-YOK2pV08E6lKo_HPVjLtL_FNi5wYIhwD8At_MsOZuudAeYlwVMdlJtdkr2UZTT-nXLhwn7XenBv5p_fekwE7oxZ5ipEP9wvdeEd8Sie9xBqAY7R3m1LEndDw5QwWc" alt="drawing" width="500"/>

## Feature 4: Generative AI - PaLM API Prompted with Store Data 




<img src="https://lh5.googleusercontent.com/Nv02RfiJxa7_48G9h2SaJmE6uRmoD41-DzzFR55aEZpR29kUYI8LI6AEEDyobxRns7iyPi-Ipm1LZe2e3YTVB_PW2VVa_aDqenWimeMxwrC-3pLHQY0Jpccy--gB9SF-zb9nA1jByED4Aox0gNZk85E" alt="drawing" width="500"/>

|                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------- |
The PaLM API consists of two APIs, each with a distinct method for generating content:

- The Chat API can be used to generate candidate `Message` responses to input messages via the `generateMessage()` function.
- The Text API can be used to generate candidate `TextCompletion` responses to input strings via the `generateText()` function.

This demo uses the Text API. If you’re looking for a demo that uses the Chat API, see [_Quick, Prompt!_](https://github.com/google/generative-ai-docs/tree/main/demos/palm/web/quick-prompt).

## How it Works

We can prime the model to behave in a certain way using a carefully crafted string of text called a __prompt__. It’s helpful to think of the model as a highly sophisticated text-completion engine: given the context we provide in our prompt, the model tries to output a feasible continuation or completion of that string.

Below is an example of a simple text prompt:

```
For each animal below, the animal's color is given.
Animal: crab
Color: red
Animal: frog
Color: green
Animal: blue jay
Color: blue
Animal: flamingo
Color:
```

If we send the above string to the model, we might expect the model to output “pink” (likely followed by additional animals and their respective colors). Adapting this prompt to generate the color of a different animal is simply a matter of replacing “flamingo” with the desired animal. Each complete (animal, color) pair in the prompt can be thought of as an __example__—it often only takes a few examples to establish a pattern that the model can follow.

_List It_ uses this same mechanism to prime the model to generate a list from a user input. You can find the prompt in `/src/lib/priming.js`.

## Requirements

- Node.js (version 18.15.0 or higher)
- Firebase project

Make sure you have either `npm` or `yarn` set up on your machine.

## Developer Setup

Although the PaLM API provides a [REST resource](https://developers.generativeai.google/api/rest/generativelanguage/models?hl=en), it is best practice to avoid embedding API keys directly into code (or in files inside your application’s source tree). If you want to call the PaLM API from the client side as we do in this demo, we recommend using a Firebase project with the Call PaLM API Securely extension enabled.

To set up Firebase:

1. Create a Firebase project at https://console.firebase.google.com.

2. Add a web app to your Firebase project and follow the on-screen instructions to add or install the Firebase SDK.

3. Go to https://console.cloud.google.com and select your Firebase project. Then go to _Security > Secret Manger_ using the left-side menu and make sure the Secret Manager API is enabled.

4. If you don’t already have an API key for the PaLM API, follow [these instructions](https://developers.generativeai.google/tutorials/setup) to get one.

5. Install the Call PaLM API Securely extension from the [Firebase Extensions Marketplace](https://extensions.dev/extensions). Follow the on-screen instructions to configure the extension.

    __NOTE__: Your project must be on the Blaze (pay as you go) plan to install the extension.

6. Enable anonymous authentication for your Firebase project by returning to https://console.firebase.google.com and selecting _Build_ in the left panel. Then go to _Authentication > Sign-in method_ and make sure _Anonymous_ is enabled.

7. Return to https://console.cloud.google.com and select your Firebase project. Click _More Products_ at the bottom of the left-side menu, then scroll down and click _Cloud Functions_. Select each function and then click _Permissions_ at the top. Add `allUsers` to the Cloud Functions Invoker role.

The above instructions assume that this demo will be used for individual/experimental purposes. If you anticipate broader usage, enable App Check in the Firebase extension during installation and see https://firebase.google.com/docs/app-check for an in-depth implementation guide.

To run the application locally:

1. Clone the repo to your local machine.

2. Run `npm i` or `yarn` in the root folder to install dependencies.

3. Add your Firebase info to `src/lib/firebase.config.js`.

4. Run `npm run dev` or `yarn dev` to start the application. The application will be served on localhost:5555. You can change the port in `vite.config.js` if desired.


**Scott’s Question 1:**

**What should I wear when hiking, and it is really hot outside?**

<img src="https://lh6.googleusercontent.com/eN2zH-PjpRiU5C8eqIVJqYRTx1EdedgT9nAMXlPv6Utp-AyaANhEDKDt4vB2w6prXvwSF6dbo29gzTjdwcY8EFuvUfdHC0Oq5DdrehgRQx9IYJExH4ZYvkaqMjdfI150G3Ytr-BWReRs9B3oLjAI5pM" alt="drawing" width="500"/>

**Scott’s Question 2:**

**And it’s raining, too**

<img src="https://lh5.googleusercontent.com/7Qx3LDjWH83m22Ql0qyNcpodA9cxuECI4bCnerAkNEBQ1r8f0N21Z0_ZMfHMXRE6BQFNZmaXqjI7kUZ_Ona-Ab4OOhk77aGB6VCuAeq3trvmlGX7vEojr71zBKYJQLp8VMoHFe2-WO7bavvdyJDpQWM" alt="drawing" width="500"/>

<img src="https://lh5.googleusercontent.com/7CMtC_c7zysNnu8A9c7ioRdcXa1berIH_lp81B3XJfz1u36Ac6Sf_le-DERK0TiSzjP37GI1WLd34j6nGcXHqHdB-A3qdF5D42FIJ87RVBy2-6JJADXIUZZW8fOi1Lz4MSct4oLNxii4VHZGugOo3Vk" alt="drawing" width="500"/>

# How to Recreate the AI/ML

The application can be built and run entirely serverless using MongoDB’s App Services. Below is the simple architecture:

 <img src="https://lh4.googleusercontent.com/zX8mS-MaGlaz2rOgqQ_tx5mSuiAL-_G7lgVWBWzelqfYlgHriY22cPEmfADmHRjdGoVkUMa5AX4tucMUEylVdXVPpqZwOGmRDY48pKFnka_KV5AMFbZFejMWwj5b4DwVnYLabfHphv-CJsIS7HRTIXQ" alt="drawing" width="600"/>

App Services Functions and Atlas Cluster Data

Both the Atlas data and the function code for MongoStore can be found in the **data-functions** branch of the repo:

<https://github.com/mongodb-developer/search-ecommerce/tree/data-functions>

#### Step 1. Prepare Data in MongoDB Atlas

Stand up an Atlas cluster. Create a database named “mongostore” with 2 collections “products” and “customers” with the .json files in the git repository.

<div class="row">
    <div class="col-md-4" markdown="1">
        <img src="https://thumbs.bfldr.com/at/t7brjfswmnrbnttc8fjp3sm?expiry=1690640345&fit=bounds&height=800&sig=MDhmZmFhZGE2NTJiMTUyNThjNmI4MDljOGE4ZDYyMzViNjA5YTc0Ng%3D%3D&width=1100" alt="drawing" width="200"/>
    </div>
    <div class="col-md-4" markdown="1">
        <h2> Database: mongostore</h2>
        <h2> Collections: </h2>
        <h3>  products</h3>
        <h3>  customers</h3>
    </div>
</div>

#### Step 2. Create Search Index named “default” on products collection 

The default dynamically mapped index will work but this one is more specific. Make sure to name the index “**default**”.

```js
{      
    "mappings":
    {    
        "dynamic": false,   
        "fields": {     
             "category":
                {  "type": "string" },     
             "main_description":
                {   "type": "string" },      
            "name":
                {  "type": "string"  }    
        }       
    }
}
```

|     |
| --- |
|     |

Atlas App Services Application - MongoStore

Still working on the backend, let’s turn towards the backend functionality.

#### Step 1. Create an App Services application. 

I named mine “MongoStore,” but it does not matter.

#### Step 2. Create HTTPS endpoints

Create 2 HTTPS Endpoints configured as follows.

1. `/products`

- POST request
- Respond with JSON result
- Calls getProductsByPage function

2. `/users`

- GET request
- Respond with JSON result
- Calls getUser function

#### Step 3. Create Functions

Create 2 functions for the corresponding endpoint functionality with the code found in the MongoStore_AppServiceApplication folder:

1. getProductsByPage
2. getUser

MongoStore - The Front End

#### Step 1. Get the Git

Finally download the code found in the git repository <https://github.com/mongodb-developer/search-ecommerce>

```
$ git clone https://github.com/mongodb-developer/search-ecommerce

$ cd search-ecommerce

$ npm install

$ npm start
```

The front end and the backend are connected via the endpoints found in the Home.js page.

![](https://lh4.googleusercontent.com/2FH9tzhLcjqybF0XXnSHJjf6Qcjw0UxZSpSQNQfo_3duMjxY08amK8eQ4dZSn5jztYO-klTuBUXszv8Zo9QjQ7nIcd8Qd7XUJebQhb4G9N8UzYx84t3KKRJH7buniMcqtlALq-si22sj0_kGmQpSvaY)

#### Step 2. Insert your own HTTPs endpoints 

Now we will need to connect our newly downloaded front end code to our newly created HTTPs endpoints.

In the front end application code, go to the src/pages/Home.js directory and replace the endpoints found around lines 52 and 55 as seen below with your own.

![](https://lh6.googleusercontent.com/cajaktS1mfQXdzitDTPwCMJrzN3drmJN_vhNcrJ5UvGARxj9NG5YOmMdIkBr-L0XOMEmoTRzypdkSV7vg7uxxVQ_fhOrZ-w55T9RJnGPHKh5zIJwyo9O7DW_0LL7LDGI1K09qEbfelTA2MFHhWVkXsI)

Step 4. Save and run

```
yarn start
```

Et voila! Log in as [karen@gmail.com](mailto:karen@gmail.com) or [scott@streammeup.com](mailto:scott@streammeup.com). Also, chat away with MongoStore. The experience will always be the same though. To customize the application to provide a different user experience, keep reading!

# How to Customize the AI/ML E-Commerce Demo

Don’t feel like being a “Karen”? Don’t worry. You can easily modify the data and the code to customize the demo for the speaker.

Key Components for Change

In the code found in the git repo, here are the components that make this demo experience easily modifiable:

1. User LogIn:
2. Chatbot.js

## Change the User and User Product Recommendations

To change the customer information and the customer product recommendations, do so in the data. Turn to Atlas in the **customers** collection.

**Sample Document:**

```js
{
    _id: ObjectId(‘63229e0ae634e04e58252a74’),
    address:{},
    email: “karen@gmail.com”,
    first_name: “Karen”,
    last_name: “Huaulme”,
    image: “https://……”,          
    cart: [
        {   name: “Super fancy product name”,
            price: 30,  
            main_image_url: ”https&#x3A;//….” }, 
            {...}, 
            {...}],
            recommendedProducts: [
                { 
                    name: “Super fancy product name”,
                    price: 30,  
                    category:  “Cosmetics”,
                    main_image_url: “https://……”,
                }, 
                {...}, 
                {...}
            ]
        },
        {...},
        {...}
    ]
}

```

1. Change the email to match what you set in the onSubmit function of the Login.js component.

2. Now you can change the user by changing the following fields:

   1. first_name
   2. last_name
   3. image

3. Change the product recommendation in the **recommendedProducts** field:

   1. name
   2. price
   3. category
   4. main_image_url

|                                                                                                                                                                                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| *Note to Presenter:**There are many different fields, but the yellow ones are the ones needed by the front end.**Price is an integer.**Image is for the user’s profile. Simply the web url of the user.**Suggest to keep no more than* *3 objects in the cart array and* - *6 objects in the recommendedProducts array.*  |

Now you need to update the front end.

In the **Login.js** Component, go to the **onSubmit** function on line 7:

```js
const onSubmit = (data) => {
    if (data.email.toLowerCase() === “[karen@gmail.com](mailto:karen@gmail.com)”
        setCurrentCustID(“63229e0ae634e04e58252a74”);
    if (data.email.toLowerCase() === “[scott@streammeup.com](mailto:scott@streammeup.com)” 
        setCurrentCustID(“63229e0ae634e04e58252a71”);
    setShowLogin(false)}
```

Hard code the login email to match what you have in the customer document in Atlas.

## Change the Chat and Chat Recommendations

We build a powerful conversational AI chatbot using Google's PaLM API 2. Learn how to set up the PaLM account, integrate the API, and create an engaging chatbot interface



```js
{
    index: 0,
    question: “What should I wear… “,
    answer: [ 
        `blah blah… `, 
        `blee blee… `,
        `bloo bloo… `
    ],
    productSuggestions: [
        {
            name: “Zion Shorts”,
            main_image_url: “https://……”,
            price: 60
        },
        {...},
        {..}
    ]
}
```

To change the responses, change the **answer** field.

The productSuggestions can be changed, as well.
