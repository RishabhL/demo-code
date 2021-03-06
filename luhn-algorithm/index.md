---
title: Luhn Algorithm
description: Replication of the Luhn algorithm
layout: default
icon: credit_card
---

<link href="style.css" rel="stylesheet" type="text/css">
<script src="script.js" type="text/javascript"></script>

# Validate Your Number
<!-- input field (in a container so that unwanted overflow from :before & :after is hidden) -->
<div class="mdc-text-field-container">
    <div class="mdc-text-field mdc-text-field--outlined"  data-mdc-auto-init="MDCTextField">
        <input type="number" id="number-input-field" class="mdc-text-field__input">
        <label for="number-input-field" class="mdc-floating-label ">Number</label>
        <div class="mdc-notched-outline">
            <svg>
                <path class="mdc-notched-outline__path"/>
            </svg>
        </div>
        <div class="mdc-notched-outline__idle"></div>
    </div>
    <!-- input field helper text -->
    <p class="mdc-text-field-helper-text" aria-hidden="true">
        Validate with the Luhn Algorithm
    </p>
</div>
<!-- button to submit & check number with Luhn algorithm -->
<button class="validation_button mdc-button mdc-button--outlined" onclick="checkNumber()" data-mdc-auto-init="MDCRipple">
    <i class="material-icons mdc-button__icon">check_circle_outline</i>
    Check
</button>
<!-- displays evaluation of number by Luhn algorithm -->
<p id="validation_message"></p>

