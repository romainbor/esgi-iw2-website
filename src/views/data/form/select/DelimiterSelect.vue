<template>
  <b-form-select
          :id="id"
          :plain="true"
          v-model="selected"
          :options="options">
  </b-form-select>
</template>

<script>
    export default {
        name: 'delimiter-select',
        components: {},
        props: [
            'id'
        ],
        data() {
            return {
                show: true,
                id: null,
                selected: null,
                options: [{
                    value: null,
                    text: 'Select a delimiter'
                }, {
                    value: 'semicolon',
                    text: ';'
                }, {
                    value: 'coma',
                    text: ','
                }]
            }
        }
    }
</script>
