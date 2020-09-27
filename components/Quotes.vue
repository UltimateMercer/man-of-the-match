<template>
  <div class="container pb-4">
    <h3 class="exo-font">
      <span class="marker marker-teal px-2">#ManOfTheMatchSeptember</span>
    </h3>
    <h3 class="exo-font text-teal my-3">Escolha a frase do mês de setembro?</h3>
    <b-form-group>
      <b-form-radio-group
        id="btn-radios-3"
        v-model="selected"
        buttons
        button-variant="special-teal"
        size="lg"
        stacked
        name="radio-btn-stacked"
        class="exo-font mt-0"
        style="width: 100% !important; display: block"
      >
        <template v-for="(option, i) in quotes">
          <b-form-radio :key="i" :value="option.value" class="text-left my-2">
            <div style="display: inline-grid !important">
              <span
                class="mb-2"
                style="
                  display: inline-grid;
                  font-weight: 400;
                  font-style: italic;
                "
              >
                "{{ option.text }}"
              </span>
              <span style="font-size: 1rem; font-style: italic">
                Por {{ option.author }}
              </span>
            </div>
          </b-form-radio>
        </template>
      </b-form-radio-group>
    </b-form-group>

    <button class="btn btn-block btn-lg btn-teal my-4">Escolher frase</button>
  </div>
</template>
<script>
export default {
  name: 'Quotes',
}
</script>
