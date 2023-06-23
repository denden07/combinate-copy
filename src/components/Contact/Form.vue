<template>
    <div class="contact-form-container">
        <div class="contact-form">
            <div class="contact-form-grid">
                <div class="form-fields-container">
                    <div class="form-fields">
                        <form action="">
                            <div class="input-fields">
                                <label for="Name" class="field-label">full name</label>
                                <input type="text" class="text-field" name="Name" placeholder="Full Name" id="Name" required="">
                            </div>
                            <div class="input-fields">
                                <label for="Email" class="field-label">Email Address</label>
                                <input type="text" class="text-field" name="Email" placeholder="Email Address" id="Name" required="">
                            </div>
                            <div class="input-fields">
                                <label for="Email" class="field-label">Work Phone</label>
                                <input type="text" class="text-field" name="Email" placeholder="Work Phone" id="Name" required="">
                            </div>
                            <div class="input-fields">
                                <select v-model="selected" id="General-Enquiry" name="General-Enquiry" data-name="General Enquiry" required="" class="text-field select w-select">
                                    <option :value="null">Select one...</option>
                                    <option value="Custom Software Development">Custom Software Development</option>
                                    <option value="Website Development">Website Development</option>
                                    <option value="AWS Technology Partner">AWS Technology Partner</option>
                                    <option value="Automation Consultancy">Automation Consultancy</option>
                                    <option value="Software Consultancy">Software Consultancy</option>
                                    <option value="UI/UX Design">UI/UX Design</option>
                                    <option value="Saas/Marketplace Development">Saas/Marketplace Development</option>
                                    <option value="Technical Documentation">Technical Documentation</option>
                                    <option value="Workflow Automation">Workflow Automation</option>
                                </select>
                            </div>
                            <div class="input-fields">
                                <label for="Email" class="field-label">Description of project</label>
                                <textarea id="Description-of-Project" name="Description-of-Project" maxlength="5000" data-name="Description of Project" placeholder="What problem are you trying to solve? When do you want it solved by?" class="textarea" spellcheck="false"></textarea>
                            </div>

                            <div class="field_block recaptcha">
                                    <div class="w-embed">
                                    </div>
                                    <div data-sitekey="6Lejie0UAAAAAFbGX-wq16eqjKEQY54rdxVydgfw" class="w-form-formrecaptcha recaptcha g-recaptcha g-recaptcha-error g-recaptcha-disabled"></div>
                                    <input type="submit" value="contact us" data-wait="Please wait..." class="button-primary w-button"/>
                                </div>
                        </form>
                    </div>
                </div>
                <div class="contact-container">
                    <h2>Contact</h2>
                    <div class="contact-list-wrapper">
                            <div class="emoji-wrapper">
                                <p class="h5 _0-padding">Say hello</p>
                                <img src="https://assets.website-files.com/5e9d4b4d716f9d3d61c9f15a/5f44973a0fbca2c607672bb7_wave%201%402x.png" height="24" alt="Hello Icon" class="emoji"/>
                            </div>
                            <a href="mailto:hello@combinate.me" class="link-block bottom-padding w-inline-block">
                                <h3 class="h3 left contact">hello@combinate.me</h3>
                            </a>
                            <a href="tel:1300247018" class="link-block bottom-padding w-inline-block">
                                <h3 class="h3 left contact">1300 247 018</h3>
                            </a>
                    </div>
                    <div class="contact-list-wrapper">
                            <div class="emoji-wrapper">
                                <p class="h5 _0-padding">Visit us</p>
                            </div>
                            <a href="https://www.google.com/maps/place/11+Wilson+St,+South+Yarra+VIC+3141,+Australia/@-37.8436983,144.9936661,17z/data=!3m1!4b1!4m5!3m4!1s0x6ad66828476f5f37:0x75d444ae6163efba!8m2!3d-37.8436983!4d144.9958548" target="_blank" class="link-block w-inline-block">
                                <h3 class="h3 left address">
                                    11 Wilson Street, <br/>
                                    South Yarra VIC 3141<br/>Australia
                                </h3>
                            </a>
                        </div>
                        <div class="map-block">
                            <div class="snazzymap lazy w-embed w-iframe">
                                <iframe src="https://snazzymaps.com/embed/234811" width="100%" height="300px" style="border:none;"></iframe>
                            </div>
                        </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    export default {

        data() {
            return {
                selected: null
            }
        }
    }
</script>

<style scoped>
.contact-form-container {
    z-index: 0;
    flex-direction: column;
    align-items: center;
    margin-top: -412px;
    margin-bottom: 104px;
    display: flex;
    position: relative;
}
.contact-form {
    opacity: 1;
    transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
    transform-style: preserve-3d;
    width: auto;
    height: auto;
    max-width: 1200px;
    min-width: 1000px;
    box-shadow: none;
    align-items: center;
    margin: 0 0% 0;
    padding: 0;
    transition-property: none;
    background-color: #fff;
    border-radius: 10px;
    flex-direction: column;
    justify-content: flex-start;
}
.contact-form-grid {
    width: auto;
    max-width: 1000px;
    min-width: 1000px;
    margin: 40px;
    padding: 0;
    grid-template-rows: auto;
    grid-template-columns: 1fr .75fr;
    grid-row-gap: 16px;
    grid-column-gap: 16px;
    grid-auto-columns: 1fr;
    display: grid;
}
.form-fields-container {
    align-self: center;
    justify-self: center;
    width: 100%;
    padding-left: 0;
    padding-right: 0;
}
.input-fields {
    width: 480px;
    margin-bottom: 24px; 
    margin-left: 0;
    padding-left: 0;
}
.field-label  {
    color: #323d53;
    letter-spacing: 1px;
    text-transform: uppercase;
    margin-bottom: 8px;
    font-family: Rubik,Arial,sans-serif;
    font-size: 10px;
    font-weight: 500;
    display: block;
}
.text-field {
    color: #08083d;
    background-color: #fff;
    border: 1px solid rgba(140,148,164,.3);
    border-radius: 4px;
    margin-bottom: 0;
    padding: 24px 16px;
    font-family: Rubik,Arial,sans-serif;
    font-size: 16px;
    font-weight: 300;
    width: 100%;
    height: 38px;
    line-height: 1.42857;
    display: block;
}
.textarea {
    height: auto;
    max-height: none;
    max-width: 480px;
    min-height: 100px;
    color: #435b8c;
    border: 1px solid rgba(140,148,164,.3);
    border-radius: 4px;
    font-family: Rubik,Arial,sans-serif;
    font-size: 16px;
    font-weight: 300;
    line-height: 24px;
    width: 100%;
    background-color: #fff;
    margin-bottom: 10px;
    padding: 8px 12px;
    display: block;
    overflow: auto;
}
.field_block .recaptcha{
    width: 480px;
    justify-content: space-between;
    align-items: flex-start;
    display: flex;
}

.field_block {
    margin-left: 0;
    padding-left: 0;
}

.w-form-formrecaptcha {
    margin-bottom: 8px;
}

input.w-button {
    -webkit-appearance: button;
}
.button-primary {
    color: #fff;
    text-align: center;
    text-transform: uppercase;
    cursor: pointer;
    background-color: #1e43ff;
    border: 1px #000;
    border-radius: 0;
    align-self: center;
    margin-top: 0;
    padding: 12px 32px;
    font-family: Rubik,Arial,sans-serif;
    font-size: 14px;
    font-weight: 400;
    text-decoration: none;
    transition: box-shadow .325s,background-color .3s,transform .2s;
    position: static;
}

.w-button {
    color: #fff;
    line-height: inherit;
    cursor: pointer;
    background-color: #3898ec;
    border: 0;
    border-radius: 0;
    padding: 9px 15px;
    text-decoration: none;
    display: inline-block;
}

.contact-container {
    width: 100%;
    padding-top: 0;
    padding-left: 24px;
    padding-right: 24px;
}

.contact-container a{
    text-decoration: none;
}
.contact-container h2 {
    font-weight: 500;
    color: #08083d;
    text-align: left;
    margin-top: 8px;
    margin-bottom: 24px;
    font-family: Rubik,Arial,sans-serif;
    font-size: 32px;
    font-weight: 400;
    line-height: 40px;
}

.contact-list-wrapper {
    flex-direction: column;
    align-items: flex-start;
    margin-bottom: 16px;
    display: flex;
}

.h3.left.contact {
    padding-top: 0;
    padding-bottom: 0;
}

.h3.left {
    color: #08083d;
    text-align: left;
    font-family: Rubik,Arial,sans-serif;
    font-weight: 400;
    text-decoration: none;
}
.contact {
    height: auto;
    background-image: linear-gradient(transparent,rgba(140,148,164,.02));
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 0;
    padding-top: 60px;
    padding-bottom: 140px;
    display: flex;
    position: static;
}
.h3 {
    color: #08083d;
    text-align: center;
    margin-top: 0;
    margin-bottom: 16px;
    padding-top: 0;
    padding-bottom: 0;
    font-family: Rubik,Arial,sans-serif;
    font-size: 18px;
    font-weight: 400;
    line-height: 26px;
}

</style>