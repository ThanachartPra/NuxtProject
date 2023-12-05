<template>
    <div class="form-contact">
        <form action="/">
            <div class="head-contact">
                <div style="font-size: 25px; margin: 2px">Contact us</div>
                <div style="font-size: 20px; margin: 2px">tell me your feedback</div>
            </div>
            <div style="display: flex;">
                <div class="main-contact">
                    <div style="text-align: center; margin: 10px;">
                        Firstname
                        <input type="text" id="firstname" name="firstname" style="width: 90%; border-radius: 5px;">
                    </div>
                    <div style="margin: 10px;">
                        Lastname
                        <input type="text" id="lastname" name="lastname" style="width: 90%; border-radius: 5px;">
                    </div>
                    <div style="margin: 10px;">
                        Email
                        <input type="email" id="email" name="email" style="width: 90%; border-radius: 5px;">
                    </div>
                </div>
                <div class="main-contact">
                    <div style="margin: 10px; margin-bottom: 0px;">Message</div>
                    <textarea name="msg" id="msg" maxlength="500" cols="29" rows="7"
                        class="descriptionArea"></textarea>
                </div>
            </div>
            <div class="foot">
                <input type="submit" value="Submit" style="border-radius: 5px;">
            </div>
        </form>
    </div>
</template>

<script setup>
useHead({
    title: 'Contact us',
    meta: [
        { name: 'description', content: 'Contact site.' }
    ]
})
</script>

<style scoped>
.form-contact {
    
    border-style: solid;
    border-color: black;
    border-radius: 10px;
    width: 500px;
    height: auto;
    text-align: center;
}

.head-contact {
    border-style: solid;
    border-radius: 10px;
    border-color: white;
    color: white;
    background-color: #333;
}

.main-contact {
    width: 49%;
    height: 160px;
    border-style: solid;
    border-radius: 10px;
    color: white;
    background-color: #333;
}

.descriptionArea {
    height: max-content;
    margin: 5px;
    margin-top: 0px;
    border-radius: 5px;
    resize: none;
}

.foot {
    background-color: #333;
    border-color: white;
    border-style: solid;
    border-radius: 10px;
    padding: 2px;
}
</style>