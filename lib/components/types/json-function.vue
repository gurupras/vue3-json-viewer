<script>
import { h } from 'vue'

export default {
  name: 'JsonFunction',
  functional: true,
  props: {
    jsonValue: {
      type: Function,
      required: true
    }
  },
  render () {
    return h('span', {
      class: {
        'jv-item': true,
        'jv-function': true
      },
      title: this.jsonValue.toString(),
      innerHTML: '&lt;function&gt;'
    })
  }
}
</script>
