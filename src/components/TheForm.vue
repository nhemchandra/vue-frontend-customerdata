<template>
  <form @submit.prevent="submitForm">
    <div class="form-control">
      <label for="first-name">First Name</label>
      <input id="first-name" name="first-name" type="text" />
    </div>
    <div class="form-control">
      <label for="last-name">Last Name</label>
      <input id="last-name" name="last-name" type="text" />
    </div>
    <div class="form-control">
      <label for="age">Your Age (Years)</label>
      <input id="age" name="age" type="number" min="19" />
    </div>
    <div class="form-control">
      <label for="children">Number of Children</label>
      <input id="children" name="children" type="number" min="0" />
    </div>
    <div class="form-control">
      <label for="Monthly income">Monthly Income in US dollars</label>
      <input id="Monthly income" name="Monthly income" type="number" min="0" />
    </div>
    <div class="form-control">
      <label for="Monthly savings">Approximate Monthly Savings in US dollars</label>
      <input id="Monthly savings" name="Monthly savings" type="number" min="0" />
    </div>
    <div class="form-control">
      <label for="Bank balance">Total Money in Bank</label>
      <input id="Bank balance" name="Bank balance" type="number" min="0" />
    </div>
        <div class="form-control">
      <h2>Credit Score</h2>
      <div>
        <input id="very poor" name="creditscore" type="radio" />
        <label for="very poor">300-579 (very-poor)</label>
      </div>
      <div>
        <input id="fair" name="creditscore" type="radio" />
        <label for="fair">580-669 (Fair)</label>
      </div>
      <div>
        <input id="good" name="creditscore" type="radio" />
        <label for="good">670-739 (Good)</label>
      </div>
      <div>
        <input id="verygood" name="creditscore" type="radio" />
        <label for="verygood">740-799 (Very Goods)</label>
      </div>
      <div>
        <input id="exceptional" name="creditscore" type="radio" />
        <label for="exceptional">800-850 (Exceptional)</label>
      </div>
    </div>
    <div class="form-control">
      <label for="assets">Approximate Total Asset value</label>
      <input id="assets" name="assets" type="number" min="0" />
    </div>
    <div class="form-control">
      <label for="liabilities">Approximate Liabilities ( loans, Alimony etc )</label>
      <input id="liabilities" name="liabilities" type="number" min="0" />
    </div>
     <div class="form-control">
      <label for="retire">Retirement Year</label>
      <input id="retire" name="retire" type="number" min="2020" max="2099" />
    </div>

  <div class="form-control">
      <label for="invest">Money will be invested in US dollars</label>
      <input id="invest" name="invest" type="number" min="0" />
    </div>

  <div class="form-control">
      <h2>Investment Tenure</h2>
      <div>
        <input id="shortterm" name="tenure" type="radio" />
        <label for="shortterm">Short Term</label>
      </div>
      <div>
        <input id="longterm" name="tenure" type="radio" />
        <label for="longterm">Long Term</label>
      </div>
    </div>

 <div class="form-control">
      <h2>Investment Style</h2>
      <div>
        <input id="agrressive" name="tenure" type="radio" />
        <label for="aggressive">Aggressive</label>
      </div>
      <div>
        <input id="moderate" name="tenure" type="radio" />
        <label for="moderate">Moderate</label>
      </div>
      <div>
        <input id="riskfree" name="tenure" type="radio" />
        <label for="riskfree">No Risk</label>
      </div>
    </div>

    <div class="form-control">
      <h2>Product Types Interested</h2>
      <div>
        <input id="banking" name="interest" type="checkbox" />
        <label for="banking">Banking</label>
      </div>
      <div>
        <input id="auto" name="interest" type="checkbox" />
        <label for="auto">Auto</label>
      </div>
      <div>
        <input id="mortgage" name="interest" type="checkbox" />
        <label for="mortgage">Mortgage</label>
      </div>
      <div>
        <input id="moneymarket" name="interest" type="checkbox" />
        <label for="moneymarket">Money Markets</label>
      </div>
      <div>
        <input id="trading" name="interest" type="checkbox" />
        <label for="trading">Self Ditrected Trading</label>
      </div>

    </div>

    <div class="form-control">
      <label for="email">Email</label>
      <input id="email" name="email" type="email" />
    </div>
    <div class="form-control">
      <label for="referrer">How did you hear about us?</label>
      <select id="referrer" name="referrer">
        <option value="google">Google</option>
        <option value="wom">Word of mouth</option>
        <option value="newspaper">Newspaper</option>
        <option value="newspaper">Facebook</option>
        <option value="newspaper">Twitter</option>
        <option value="newspaper">TV Commercial</option>
      </select>
    </div>

    
    <div>
      <button>Submit</button>
    </div>
  </form>
</template>


<script>
export default {
  methods: {
      submitForm() {}
  }

}
</script>


<style scoped>
form {
  margin: 2rem auto;
  max-width: 40rem;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.26);
  padding: 2rem;
  background-color: #ffffff;
}

.form-control {
  margin: 0.5rem 0;
}

label {
  font-weight: bold;
}

h2 {
  font-size: 1rem;
  margin: 0.5rem 0;
}

input,
select {
  display: block;
  width: 100%;
  font: inherit;
  margin-top: 0.5rem;
}

select {
  width: auto;
}

input[type='checkbox'],
input[type='radio'] {
  display: inline-block;
  width: auto;
  margin-right: 1rem;
}

input[type='checkbox'] + label,
input[type='radio'] + label {
  font-weight: normal;
}

button {
  font: inherit;
  border: 1px solid #0076bb;
  background-color: #0076bb;
  color: white;
  cursor: pointer;
  padding: 0.75rem 2rem;
  border-radius: 30px;
}

button:hover,
button:active {
  border-color: #002350;
  background-color: #002350;
}
</style>