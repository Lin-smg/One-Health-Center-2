<template>
<table class="table">
    <thead>
      <slot name="columns">
        <tr>
          <th v-for="column in columns" :key="column.key">{{column.label}}</th>
        </tr>
      </slot>
    </thead>
    <tbody>
    <tr v-for="(item, index) in data" :key="index">
      <slot :row="item">
        <td v-for="column in columns" :key="column" v-if="hasValue(item, column)">{{itemValue(item, column)}}</td>
      </slot>
    </tr>
    </tbody>
  </table>
</template>

<script>
export default {
    name: "custom-table"
}
</script>