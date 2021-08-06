https://codesandbox.io/s/elegant-moon-nc092


import React from "react";
import ReactDOM from "react-dom";
import App from "./components/App";

ReactDOM.render(
  <div>
    <App />
  </div>,
  document.getElementById("root")
);

import React from "react";
import Header from "./Header";
import Footer from "./Footer";
import Netflix from "./Netflix";
import Python from "./Python";

function App() {
  return (
    <div>
      <Header />
      <Netflix />
      <Python />
      <Footer />
    </div>
  );
}

export default App;

import React from "react";
function Footer() {
  var currYear = new Date().getFullYear();

  return (
    <footer>
      <p>Copyright @ {currYear}</p>
    </footer>
  );
}

export default Footer;


import React from "react";
function Header() {
  return (
    <header>
      <h1>ShapeAI</h1>
    </header>
  );
}

export default Header;


import React from "react";

function Netflix() {
  return (
    <div className="note">
      <h1>Netflix Clone Bootcamp</h1>
      <p>
        Shape AI is now conducting a 7 day bootcamp on building basic netflix
        clone. The bootcamp is conducted by Mr.Pavan KP which started from 26 of
        July.
      </p>
    </div>
  );
}

export default Netflix;

import React from "react";

function Python() {
  return (
    <div className="note">
      <h1>Python and Cloud Security Bootcamp</h1>
      <p>
        Shape AI is now conducting a 7 day bootcamp on Python and Cloud
        Security. The bootcamp is conducted by Mr.Harsh Akshith which started
        from 26 of July.
      </p>
    </div>
  );
}

export default Python;

