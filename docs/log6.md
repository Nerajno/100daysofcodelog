---
title: 100 Days of Code - Round 1
description: by [Your Name]
#pg_bk_color: '#e6e8de'
#header_bk_color: '#1a7f6d'
#link_color: '#1a7f6d'
---
<!-- markdownlint-disable MD022 MD024 MD032 MD033 -->

# 100 Days of Code
<p class="toc"><a href="./index.html">&lt;– back to Table of Contents</a></p>

| Log 1 | Log 2 | Log 3 |
| --- | --- | --- |
| this log | [100 Days Round 2](log2.html) | [100 Days Round 3](log3.html) |

## Challenge & Commitment
This is part of Alexander Kallaway's [100DaysOfCode](https://github.com/Kallaway/100-days-of-code "the official repo") challenge. More details about the challenge can be found here: [100daysofcode.com](http://100daysofcode.com/ "100daysofcode.com").

**Commitment:** *I will code daily for the next 100 days.*

|  Start Date   | End Date     |
| ------------- | ------------ |
| Today's date  | - - - |

## Goals

- [x] Code daily
- [ ] Goal 2
- [ ] Goal 3

# Code Log

---

<<<<<<< HEAD
## 1. Sample Entry
### Day 1: February 26, 2019 - Tuesday
=======
## 31. Checkout Page
### Day 31: August 30, 2019 - Friday

**Project:** [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

[![App](assets/images/r6d31-small.jpg)](assets/images/r6d31.jpg)<br>
<span class="center bold">Checkout Page</span>

**Progress:**

In this lesson I built the cart page which allows the quantity to be updated and also allows removing of items from the cart.

This was done with

- Redux Actions
- Redux Reducers
- Utility functions

The cartItem component looks like this.

```jsx
import React from 'react';
import { connect } from 'react-redux';

import {
  addItem,
  removeItem,
  clearItemFromCart
} from '../../redux/cart/cart.actions';

import './checkout-item.styles.scss';

const CheckoutItem = ({ cartItem, clearItem, addItem, removeItem }) => {
  const { name, imageUrl, price, quantity } = cartItem;
  return (
    <div className="checkout-item">
      <div className="image-container">
        <img src={imageUrl} alt="item" />
      </div>
      <span className="name">{name}</span>
      <span className="quantity">
        <div className="arrow" onClick={() => removeItem(cartItem)}>
          &#10094;
        </div>
        <span className="value">{quantity}</span>
        <div className="arrow" onClick={() => addItem(cartItem)}>
          &#10095;
        </div>
      </span>
      <span className="price">{price}</span>
      <span className="remove-button" onClick={() => clearItem(cartItem)}>
        &#10005;
      </span>
    </div>
  );
};

const mapDispatchToProps = dispatch => ({
  clearItem: item => dispatch(clearItemFromCart(item)),
  addItem: item => dispatch(addItem(item)),
  removeItem: item => dispatch(removeItem(item))
});

export default connect(
  null,
  mapDispatchToProps
)(CheckoutItem);
```

**Links:**
- My GitHub Repo - [Crown Clothing Repo](https://github.com/james-priest/crown-clothing)
- [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

---

## 30. Cart Display
### Day 30: August 28, 2019 - Wednesday

**Project:** [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

[![App](assets/images/r6d30-small.jpg)](assets/images/r6d30.jpg)<br>
<span class="center bold">Cart Display</span>

**Progress:**

This lesson dealt with creating the CartItem component to display products added to the cart.

It uses the connect() method of 'react-redux' to access the store.

[![App](assets/images/r6d30a-small.jpg)](assets/images/r6d30a.jpg)<br>
<span class="center bold">Card Display with Redux store</span>

**Links:**
- My GitHub Repo - [Crown Clothing Repo](https://github.com/james-priest/crown-clothing)
- [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

---

## 29. Add Items to Cart
### Day 29: August 27, 2019 - Tuesday

**Project:** [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

[![App](assets/images/r6d29-small.jpg)](assets/images/r6d29.jpg)<br>
<span class="center bold">Redux Logger</span>

**Progress:**

In this lesson we learned how to add items to our Redux shopping cart.

[![App](assets/images/r6d29a-small.jpg)](assets/images/r6d29a.jpg)<br>
<span class="center bold">Items added to cart</span>

This is displayed in our Redux logger.

Multiple items are handled with a cart utility function.

[![App](assets/images/r6d29b-small.jpg)](assets/images/r6d29b.jpg)<br>
<span class="center bold">Utility function in reducer</span>

**Links:**
- My GitHub Repo - [Crown Clothing Repo](https://github.com/james-priest/crown-clothing)
- [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

---

## 28. Display Product Items
### Day 28: August 26, 2019 - Monday

**Project:** [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

[![App](assets/images/r6d28-small.jpg)](assets/images/r6d28.jpg)<br>
<span class="center bold">Product Items</span>

**Progress:**

This lesson dealt with setting up the display of products and creating buttons on items to add them to the shopping cart.

[![App](assets/images/r6d28a-small.jpg)](assets/images/r6d28a.jpg)<br>
<span class="center bold">Add Item to cart</span>

**Links:**
- My GitHub Repo - [Crown Clothing Repo](https://github.com/james-priest/crown-clothing)
- [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

---

## 27. Add Redux Boilerplate
### Day 27: August 24, 2019 - Saturday

**Project:** [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

[![App](assets/images/r6d27-small.jpg)](assets/images/r6d27.jpg)<br>
<span class="center bold">Redux Flow</span>

**Progress:**

This set of lessons was all about setting up Redux boilerplate into an existing app.

Middleware was set up for Redux logging.

[![App](assets/images/r6d27b-small.jpg)](assets/images/r6d27b.jpg)<br>
<span class="center bold">Redux Logger</span>

The nice thing that this lesson focused on was proper organization of items for large-scale applications.

It included:

- Types & constants
- Action creators
- Reducers
- Middleware

[![App](assets/images/r6d27a-small.jpg)](assets/images/r6d27a.jpg)<br>
<span class="center bold">VS Code</span>

**Links:**
- My GitHub Repo - [Crown Clothing Repo](https://github.com/james-priest/crown-clothing)
- [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

---

## 26. Firebase Firestore
### Day 26: August 22, 2019 - Thursday

**Project:** [Complete React Developer in 2019 (w/ Redux, Hooks, GraphQL)](https://www.udemy.com/complete-react-developer-zero-to-mastery/) - Neagoie & Zhang

[![App](assets/images/r6d26-small.jpg)](assets/images/r6d26.jpg)<br>
<span class="center bold">Firebase Firestore</span>

**Progress:**

Today I implemented two forms of Firebase Authentication:

- Sign In with Google (OAuth)
- Email & Password Sign In

I also started working with Firestore which is a NoSQL database that allows saving of:
>>>>>>> e152888ec606ed0978802f49643523d6a6c29730

**Project:** Code Log Template

[![new code log](assets/images/day1-small.jpg)](assets/images/day1.jpg)

**Progress:** Created a new GitHub repo for my code log.

This repo is redesigned so that it can be forked and cloned for others to use. I'm still in the process of writing out the README to cover the following areas

- installation
- usage
- customization
- image optimization
- set-up & testing

**Links:** My GitHub repo [https://github.com/james-priest/100-days-log](https://github.com/james-priest/100-days-log)

---

## 2. Entry Title
### Day 2: Date - Day

**Project:**

**Progress:**

**Links:**

---

## 3. Entry Title
### Day 3: Date - Day

**Project:**

**Progress:**

**Links:**

---
