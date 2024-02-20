# jpmc-react-feb



https://1drv.ms/f/s!AkmCyIRDVU7YibwAiSt7J9MaFT6iWQ?e=yeZcyn



NOtes: Day-1


MPA-> SPA (Single Page Application)

Es6.0 
React-> 18

Component (View) Centric Application   -> JSX

JSX->javascript syntax extension

NodeJS -> platform

npm i -g create-react-app

 create-react-app my-app

cd my-app
npm  start

compile  Es6-> JS (babel)

Webpack => bundling tool


class based
functional

--------------------------

props (ReadOnly) (used in child component to get the data from parent)
event
state-> (mutable)

1)init the state
2)render the state
3)update the state
4)rerender the state


----


task-1

create a new component name counterapp

create 3 buttons and subsq methods (inc,dec,reset)

and call the methods by clicking on the buttons. and show the alert msg




------------------

Lifecycle






---------------


import React, { Component } from "react";

export default class Lsp extends Component {
  render() {
    return (
      <div>
        Welcome to Product Order Screen
        <hr/>
        <Order />
        <hr/>
        <Address />
        <hr/>
        <Summary />
      </div>
    );
  }
}

class Order extends Component {
  render() {
    return <div>
<p>Product Name 
    <select>
        <option>Product-1</option>
        <option>Product-2</option>
        <option>Product-3</option>
    </select>
</p>
<p>Enter Quantity:<input type="text" /></p>
    </div>;
  }
}

class Address extends Component {
  render() {
    return <div>
        <p>Adreess Details</p>
        Address:
        <input />
    </div>;
  }
}

class Summary extends Component {
  render() {
    return <div>
       <p> Order Summary</p>
       <p>Product Name: </p>
       <p>Update Quantity:<input type="text" /></p>
       <p>Address:</p>

    </div>;
  }
}
