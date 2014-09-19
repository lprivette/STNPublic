/* 
    Copyright 2012 USGS WiM
*/

/*
    Author: Nick Estes
    Created: December 14, 2012
*/
define([
    "dojo/_base/declare",
    "dijit/_WidgetBase",
    "dijit/_TemplatedMixin",
    "dijit/_OnDijitClickMixin",
    "dijit/_Container",
    "dojo/dom-construct",
    "dojo/dom-style",
    "dojo/parser",
    "dojo/ready",
    "dojo/text!./templates/Disclaimer.html"  
], function(
    declare,
    _WidgetBase, 
    _TemplatedMixin,
    _OnDijitClickMixin,
    _Container,
    domConstruct,
    domStyle,
    parser,
    ready,
    template
) {
     return declare( "wim/Disclaimer", [_WidgetBase, _TemplatedMixin], {

        templateString: template,
        //declaredClass: "wim/Disclaimer",
        baseClass: "disclaimer",
        attachedMapID: null,
    
        constructor: function () {

            console.log("Disclaimer wijit created");
        
        },

        postCreate: function () {

            var domNode = this;
            
            var horCenter = domStyle.get(document.body, "width") / 2;
            var vertCenter = domStyle.get(document.body, "height") / 2;
            var disclaimerWidth = domStyle.get(this.id, "width") / 2;
            var disclaimerHeight = domStyle.get(this.id, "height") / 2;
            domStyle.set(this.id, 'left', horCenter - disclaimerWidth + "px");
            domStyle.set(this.id, 'top', vertCenter - disclaimerHeight + "px");
            
        },

        _onChange: function () {
           
        }
     });

     ready(function() {
        parser.parse();

     });
});