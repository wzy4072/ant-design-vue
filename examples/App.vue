<template>
  <div>
    <a-layout>
      <a-layout-header>Header</a-layout-header>
      <a-layout-content>
        <TableDemo1></TableDemo1>
      </a-layout-content>
      <a-layout-footer>Footer</a-layout-footer>
    </a-layout>
  </div>
</template>
<script>
import { defineComponent } from 'vue';
// import demo from '../antdv-demo/docs/affix/demo';
// import Affix from '../components/affix';
import TableDemo1 from '../antdv-demo/TableDemo1/index';
export default defineComponent({
  components: {
    TableDemo1,
    // demo,
    // Affix,
  },
  data() {
    return {
      visible: false,
      pStyle: {
        fontSize: '16px',
        color: 'rgba(0,0,0,0.85)',
        lineHeight: '24px',
        display: 'block',
        marginBottom: '16px',
      },
      pStyle2: {
        marginBottom: '24px',
      },
    };
  },
  methods: {
    showDrawer() {
      this.visible = true;
    },
    onClose() {
      this.visible = false;
    },
  },
});
</script>
