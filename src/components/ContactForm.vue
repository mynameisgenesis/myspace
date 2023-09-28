<template>
  <div class="card mb-4" id="contact-form">
    <div class="card-header">
      <h4 class="my-0 font-weight-normal">Contact me</h4>
    </div>
    <div class="card-body">
      <form @submit="sendEmail">
        <div class="form-group row">
          <label for="email" class="col-sm-2 col-form-label"
            ><img
              src="../assets/win95/icons/envelope_closed-1.png"
              class="icon-16-4"
            />
            Your e-mail:</label
          >
          <div class="col-sm-10">
            <input type="email" class="form-95" id="email" />
          </div>
        </div>
        <div class="form-group row">
          <label for="name" class="col-sm-2 col-form-label"
            ><img
              src="../assets/win95/icons/user_world-0.png"
              class="icon-16-4"
            />
            Your name:</label
          >
          <div class="col-sm-10">
            <input type="text" class="form-95" id="name" />
          </div>
        </div>
        <div class="form-group">
          <label for="message-textarea">Message</label>
          <textarea class="form-95" id="message-textarea" rows="3"></textarea>
        </div>
        <div class="form-group row">
          <div class="col-sm-10">
            <button type="submit" class="btn btn-primary">Send</button>
          </div>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactForm",
  methods: {
    sendEmail(event) {
      console.log(event.target.value);
    },
  },
};
</script>

<style scoped>
#contact-form {
  font-family: "MS Sans Serif", Tahoma, Verdana, Segoe, sans-serif;
  padding-bottom: 28px;
}
#message {
  height: 250px;
}

/*

    Button styles

*/
.btn {
  border-width: 2px;
  border-style: outset;
  border-color: buttonface;
  border-right-color: #424242;
  border-bottom-color: #424242;
  background: silver;
  color: black;
  padding: 0 0 4px;
  border-radius: 1px;
}
.btn:hover {
  border: 2px inset #fff;
  background: silver;
  color: #424242;
  box-shadow: -1px -1px #000;
}
.btn:focus {
  border: 2px inset #fff !important;
  background: silver;
  color: #424242;
  box-shadow: -1px -1px #000 !important;
  outline: 0 !important;
  background: url(../assets/win95/background.bmp);
}
.btn:active {
  border: 2px inset #fff !important;
  color: #424242;
  box-shadow: -1px -1px #000 !important;
  outline: 0 !important;
  background: url(../assets/win95/background.bmp);
}

.btn-primary {
  padding-left: 8px;
  padding-right: 8px;
}
button:focus {
  outline: 1px dotted;
}
.btn.disabled,
.btn:disabled {
  cursor: default;
  background-color: silver;
  border-style: outset;
  border-color: buttonface;
  border-right-color: #424242;
  border-bottom-color: #424242;
  color: grey;
  text-shadow: 1px 1px #fff;
}

/*CARDS*/

.card {
  border: solid;
  border-width: 2px;
  border-bottom-color: #424242;
  border-right-color: #424242;
  border-left-color: #fff;
  border-top-color: #fff;
  background: silver;
  color: #212529;
}
.card.square {
  border-radius: 0px;
}
.card.square .card-header {
  border-radius: 0px;
}
.card.w95 .card-header {
  background: #08216b;
  /* OR #000082 is better?*/
}
.card-header {
  background: -webkit-linear-gradient(left, #08216b, #a5cef7);
  color: #fff;
  display: block;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  padding-top: 2px;
  padding-bottom: 1px;
  text-align: left;
}
.card-header.icon {
  padding-left: 4px;
}
.header-inactive {
  background: gray !important;
}

/*

FORMS

*/
.form-95 {
  width: 100%;
  border: 2px inset #d5d5d5;
  color: #424242;
  background: #fff;
  box-shadow: -1px -1px 0 0 #828282;
  margin-top: 4px;
  padding-left: 2px;
}
.bootstrap-select,
textarea:focus,
textarea.form-control:focus,
input.form-control:focus,
input[type="text"]:focus,
input[type="password"]:focus,
input[type="email"]:focus,
input[type="number"]:focus,
[type="text"].form-control:focus,
[type="password"].form-control:focus,
[type="email"].form-control:focus,
[type="tel"].form-control:focus,
[contenteditable].form-control:focus {
  outline: 0 !important;
}
input[type="radio"],
input[type="checkbox"] {
  position: absolute;
  left: -9999px;
}

.form-check-label::before,
.form-check-label::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
}
.form-check-label {
  margin-left: 6px;
}

input[type="radio"] + .form-check-label::before,
input[type="radio"] + .form-check-label::after {
  border-radius: 50%;
}

.form-check-label::before {
  height: 20px;
  width: 20px;
  top: 3px;
  padding-right: 2px;
  border: 2px inset #d5d5d5;
  background: white;
  box-shadow: -1px -1px 0 0 #828282;
}
input[type="radio"] + .form-check-label::after {
  display: none;
  width: 8px;
  height: 8px;
  margin: 6px;
  top: 3px;
  background: black;
}
input[type="checkbox"] + .form-check-label::after {
  display: none;
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23000' d='M6.564.75l-3.59 3.612-1.538-1.55L0 4.26 2.974 7.25 8 2.193z'/%3e%3c/svg%3e");
  width: 12px;
  height: 12px;
  margin: 4px;
  top: 3px;
}
input:checked + .form-check-label::after {
  display: block;
}
/**/
</style>
