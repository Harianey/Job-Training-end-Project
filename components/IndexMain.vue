<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer" app>
      <v-list color="transparent">
        <v-list-item
          prepend-icon="mdi-format-list-checks"
          title="To do"
          to="/IndexMain"
        ></v-list-item>
        <v-list-item
          prepend-icon="mdi-information-outline"
          title="About"
          to="/about"
        ></v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Final Project</v-toolbar-title>
    </v-app-bar>

    <v-main class="d-flex mb-6 bg-surface-variant">
      <v-card max-width="auto">
        <v-container>
          <v-row dense>
            <v-card-title class="text-h5"> In Progress </v-card-title>
            <v-col cols="12">
              <v-card>
                <v-card-subtitle
                  >Design Project Task. Lorem ipsum dolor sit amet, consectetur
                  adipisicing elit. Corporis ipsum distinctio, consequuntur
                  labore eveniet quaerat sit quos voluptatem ducimus ipsa quia
                  quo adipisci ea minus quam soluta. Provident, earum
                  magni!</v-card-subtitle
                >

                <v-card-text class="py-0">
                  <v-row align="center" no-gutters>
                    <v-icon
                      class="me-1"
                      icon="mdi-clipboard-text-clock-outline"
                    ></v-icon>
                    <v-list-item-subtitle>25/07/2023</v-list-item-subtitle>

                    <v-col cols="7" class="text-right">
                      <v-icon
                        class="me-1"
                        icon="mdi-trash-can-outline"
                        @click="toggleDelete"
                      ></v-icon>
                      <v-icon
                        class="me-1"
                        icon="mdi-pencil-outline"
                        @click="editTask(task)"
                      ></v-icon>
                    </v-col>
                  </v-row>
                </v-card-text>

                <v-divider></v-divider>

                <div align="center" class="my-4 text-subtitle-1">Design</div>
              </v-card>
            </v-col>

            <v-col cols="12">
              <v-card>
                <v-card-subtitle
                  >Add in div between the v-card.</v-card-subtitle
                >

                <v-card-text class="py-0">
                  <v-row align="center" no-gutters>
                    <v-icon
                      class="me-1"
                      icon="mdi-clipboard-text-clock-outline"
                    ></v-icon>
                    <v-list-item-subtitle>25/07/2023</v-list-item-subtitle>

                    <v-col cols="7" class="text-right">
                      <v-icon
                        class="me-1"
                        icon="mdi-trash-can-outline"
                        @click="toggleDelete"
                      ></v-icon>
                      <v-icon
                        class="me-1"
                        icon="mdi-pencil-outline"
                        @click="editTask(task)"
                      ></v-icon>
                    </v-col>
                  </v-row>
                </v-card-text>

                <v-divider></v-divider>

                <div align="center" class="my-4 text-subtitle-1">Code</div>
              </v-card>
            </v-col>
            <v-card-actions>
              <v-btn variant="outlined"> Add Task </v-btn>
            </v-card-actions>
          </v-row>
        </v-container>
      </v-card>
      <v-card max-width="auto">
        <v-container>
          <v-row dense>
            <v-card-title class="text-h5"> Review </v-card-title>
            <v-col cols="12">
              <v-card>
                <v-card-subtitle
                  >Semicolon missing between Lorem ipsum dolor sit amet
                  consectetur adipisicing elit. Provident iusto dolorem soluta
                  aliquid harum suscipit, sit saepe porro, ullam qui impedit
                  necessitatibus perferendis, velit odit corporis labore eius?
                  Est, at!</v-card-subtitle
                >

                <v-card-text class="py-0">
                  <v-row align="center" no-gutters>
                    <v-icon
                      class="me-1"
                      icon="mdi-clipboard-text-clock-outline"
                    ></v-icon>
                    <v-list-item-subtitle>25/07/2023</v-list-item-subtitle>

                    <v-col cols="7" class="text-right">
                      <v-icon
                        class="me-1"
                        icon="mdi-trash-can-outline"
                        @click="toggleDelete"
                      ></v-icon>
                      <v-icon
                        class="me-1"
                        icon="mdi-pencil-outline"
                        @click="editTask(task)"
                      ></v-icon>
                    </v-col>
                  </v-row>
                </v-card-text>

                <v-divider></v-divider>

                <div align="center" class="my-4 text-subtitle-1">Code</div>
              </v-card>
            </v-col>

            <v-card-actions>
              <v-btn variant="outlined"> Add Task </v-btn>
            </v-card-actions>
          </v-row>
        </v-container>
      </v-card>
      <v-card max-width="auto">
        <v-container>
          <v-row dense>
            <v-card-title class="text-h5"> Done </v-card-title>
            <v-col cols="12">
              <v-card>
                <v-card-subtitle
                  >Design Project Task. Lorem ipsum dolor sit amet, consectetur
                  adipisicing elit. Corporis ipsum distinctio, consequuntur
                  labore eveniet quaerat sit quos voluptatem ducimus ipsa quia
                  quo adipisci ea minus quam soluta. Provident, earum
                  magni!</v-card-subtitle
                >

                <v-card-text class="py-0">
                  <v-row align="center" no-gutters>
                    <v-icon
                      class="me-1"
                      icon="mdi-clipboard-text-clock-outline"
                    ></v-icon>
                    <v-list-item-subtitle>25/07/2023</v-list-item-subtitle>

                    <v-col cols="7" class="text-right">
                      <v-icon
                        class="me-1"
                        icon="mdi-trash-can-outline"
                        @click="toggleDelete"
                      ></v-icon>
                      <v-icon
                        class="me-1"
                        icon="mdi-pencil-outline"
                        @click="editTask(task)"
                      ></v-icon>
                    </v-col>
                  </v-row>
                </v-card-text>

                <v-divider></v-divider>

                <div align="center" class="my-4 text-subtitle-1">Design</div>
              </v-card>
            </v-col>

            <v-card-actions>
              <v-btn variant="outlined"> Add Task </v-btn>
            </v-card-actions>
          </v-row>
        </v-container>
      </v-card>
    </v-main>
  </v-app>
</template>

<script setup>
import { ref } from "vue";

const drawer = ref(null);
</script>

<script>
export default {
  data: () => ({ drawer: null }),
};
</script>

<!-- <script>
  methods : {
    editTask(task) {
      // Implement the logic to edit a task
      // alert(task.date)
      this.$swal.fire({
        title: 'Create a task',
        showCancelButton: true,
        confirmButtonText: 'Save Task',
        showLoaderOnConfirm: true,
        width: 600,
        html:
            '<input id="title-input" type="text" value="'+task.title+'" class="swal2-input" placeholder="enter Task Title">' +
            '<input id="date-input" type="date" value="'+task.date+'" class="swal2-input ">'+
            '<select id="type-input" class="swal2-input shadow">'+
            ' <option value="'+task.type+'">choose a type</option>'+
            ' <option value="design">Design</option>' +
            ' <option value="QA">Q&A</option>' +
            ' <option value="Feature Request">Feature Request</option>' +
            '</select>',
        preConfirm: function () {
          return new Promise(function (resolve) {
            resolve([
              document.getElementById("title-input").value,
              document.getElementById("date-input").value,
              document.getElementById("type-input").value,
            ])
          })
        },
      }).then((result) => {
        if (result) {
          task.title = result.value[0];
          task.date = result.value[1];
          task.type = result.value[2];
          this.$swal.fire(
              'Updated!',
              'The Task was updated.',
              'success'
          )
        }
      })
    },
    toggleDelete() {
      this.$emit('toggle-delete');
    }
  }
};
</script> -->
