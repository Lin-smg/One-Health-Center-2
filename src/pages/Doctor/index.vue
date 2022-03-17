<template>
  <section>

    <div class="row">
      <div class="col-lg-12 grid-margin stretch-card">
        <div class="card">
          <div class="card-body">
            <!-- <h4 class="card-title">Striped And Hoverable Table</h4>
            <p class="card-description">
              Use <code>hover striped</code> props for striped and hoverable styles
            </p> -->
            <b-table
              striped
              hover
              responsive
              :items="items"
              :fields="fields"
            ></b-table>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
const itemsTwo = [
  { Status: true, age: 40, first_name: "Dickerson", last_name: "Macdonald" },
  { Status: false, age: 21, first_name: "Larsen", last_name: "Shaw" },
  {
    Status: false,
    age: 89,
    first_name: "Geneva",
    last_name: "Wilson",
    _rowVariant: "danger",
  },
  {
    Status: true,
    age: 40,
    first_name: "Thor",
    last_name: "Macdonald",
    _cellVariants: { Status: "success", age: "info", first_name: "warning" },
  },
  { Status: false, age: 29, first_name: "Dick", last_name: "Dunlap" },
];
export default {
  name: "basicTables",
  data() {
    return {
      itemsTwo: itemsTwo,
      items: [
        {
          id: "1",
          name: "Doctor Name",
          phone: "0988776667",
          speciality: "heart",
          room: "1",
          image: "1646817573.jpg",
          created_at: "2022-03-09 09:19:34",
          updated_at: "2022-03-09 09:19:34",
        },
        {
          id: "3",
          name: "Dr. kyaw Kyi",
          phone: "0999999",
          speciality: "skin",
          room: "111",
          image: "1646819727.jpg",
          created_at: "2022-03-09 09:55:27",
          updated_at: "2022-03-10 03:20:50",
        },
        {
          id: "4",
          name: "Dr.Aye",
          phone: "0999999",
          speciality: "skin",
          room: "101",
          image: "1646882822.jpg",
          created_at: "2022-03-10 03:27:02",
          updated_at: "2022-03-10 03:27:02",
        },
        {
          id: "5",
          name: "Dr. Henry",
          phone: "09887768990",
          speciality: "heart",
          room: "102",
          image: "1647248807.jpg",
          created_at: "2022-03-14 09:06:47",
          updated_at: "2022-03-14 09:06:47",
        },
      ],
      fields: [
        {
          key: "image",
          label: "Image",
          sortable: true,
        },
        {
          key: "name",
          label: "Name",
          sortable: true,
        },
        {
          key: "phone",
          label: "Phone",
          sortable: true,
        },
        {
          key: "email",
          label: "Email",
          sortable: true,
        },
        {
          key: "speciality",
          label: "Speciality",
          sortable: true,
        },
        {
          key: "room",
          label: "Room No",
          sortable: true,
        },
      ],
    };
  },
};
</script>
