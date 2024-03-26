<script setup lang="ts">
var show = true
var classroom = 5
</script>

<template>
  <template v-if="show">
    <v-main style="height: 100vh">
      <template v-if="classroom">
        <div class="classroom-card-container">
          <v-card title="Card title" subtitle="Subtitle" text="...">
            <v-card-actions>
              <v-btn>Click me</v-btn>
            </v-card-actions>
          </v-card>
        </div>
      </template>
    </v-main>
  </template>
</template>

<style scoped>
.classroom-card-container {
  margin-top: 1rem;
  margin-left: 1rem;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 1rem;
}
</style>
