translate.js
============

A jQuery plugin to translate text in the client side.

This version has been tweaked from the original version to also support placeholder attributes for input forms.

## Usage
Step 1: include JQuery and translate.js in your page

    <script src="jquery.js"/>
    <script src="jquery.translate.js"/>

Step 2: every text you want translated include the trn class

    <span class="trn">text to translate</span>

Step 3: create your dictionary

    var dict = {
      "Home": {
        pt: "Início"
      },
      "Download plugin": {
         pt: "Descarregar plugin",
         en: "Download plugin"
      }
    }

Step 4: initialize the plugin and translate the entire page body

    var translator = $('body').translate({lang: "en", t: dict}); //use English

Step 5: change to another language

    translator.lang("pt"); //change to Portuguese

## License
You may use translate.js under the terms of the MIT License. [More information](http://en.wikipedia.org/wiki/MIT_License).
