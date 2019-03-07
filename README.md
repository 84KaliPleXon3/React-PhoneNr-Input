<h1 align="center">React-PhoneNr-Input</h1>

<div align="center">

[![NPM](https://img.shields.io/npm/v/react-phonenr-input.svg)](https://www.npmjs.com/package/react-phonenr-input)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-Airbnb-brightgreen.svg)](https://github.com/airbnb/javascript)
[![license](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/KaiHotz/react-formik-ui/blob/master/LICENSE)

</div>

## Overview
React-PhoneNr-Input is a simple to use phone number input field with country selection, that by default, intuitively guesses the country for- and formats the entered phone number

By passing the prop `format='NATIONAL'` and a default country e.g. `defaultCountry='de'`  a simple input field is shown that formats the entered phone number with the national format used by the default country specified.

All written with around then 300 lines of code


### Demo and Examples [here](https://kaihotz.github.io/React-PhoneNr-Input/)


## Installation
npm:
```sh
npm install --save react-phonenr-input
```

yarn:
```sh
yarn add react-phonenr-input
```

#### Props:
<table style="font-size: 12px">
  <tr>
    <th>Name</th>
    <th>Type</th>
    <th>Default</th>
    <th>Description</th>
  </tr>
    <tr>
    <td>name</td>
    <td>string</td>
    <td>Required</td>
    <td>Sets the Name of the Phone Nr. Input Field</td>
  </tr>
  <tr>
    <td>onChange</td>
    <td>function</td>
    <td>required</td>
    <td>The function/method that returns the entered Phone Nr.</td>
  </tr>
  <tr>
    <td>buttonFlagStyles</td>
    <td>object</td>
    <td>null</td>
    <td>Style object that overrides the styles of the Flag shown in the button</td>
  </tr>
  <tr>
    <td>className</td>
    <td>string</td>
    <td>null</td>
    <td>Adds a custom class to the Phone Nr. Input Field wrapper div</td>
  </tr>
  <tr>
    <td>defaultCountry</td>
    <td>string</td>
    <td>null</td>
    <td>Sets the default country</td>
  </tr>
  <tr>
    <td>disabled</td>
    <td>boolean</td>
    <td>false</td>
    <td>Disables the Phone Nr. Input Field</td>
  </tr>
  <tr>
    <td>format</td>
    <td>string</td>
    <td>'INTERNATIONAL'</td>
    <td>Sets the format of the entered  phone number, in case of 'NATIONAL' the defaultCountry must be set</td>
  </tr>
  <tr>
    <td>id</td>
    <td>string</td>
    <td>null</td>
    <td>Sets an Id for the Phone Nr. Input Field, if not passed, the id will be the name</td>
  </tr>
  <tr>
    <td>listFlagStyles</td>
    <td>object</td>
    <td>null</td>
    <td>Style object that overrides the styles of the Flag shown in the country dropdown</td>
  </tr>
  <tr>
    <td>placeholder</td>
    <td>string</td>
    <td>null</td>
    <td>Sets the Placeholder text</td>
  </tr>
  <tr>
    <td>preferredCountries</td>
    <td>Array</td>
    <td>null</td>
    <td>Lets you restrict the country dropdown to a specific list of countries</td>
  </tr>
  <tr>
    <td>regions</td>
    <td>String / Array</td>
    <td>[]</td>
    <td>Lets you restrict the country dropdown to a list of countries in the specified regions</td>
  </tr>
</table>



#### Code example:
```jsx
import React, { Component } from 'react'
import { PhoneInput } from 'react-phonenr-input';

class Example extends Component {

  handleChange = phoneNumber => {
    // here you hanlde the returned Phone Nr.
  }

  render () {
    return (
      <div>
        <PhoneInput name='phoneInput' onChange={handleChange}/>
      </div>
    )
  }
}
```








