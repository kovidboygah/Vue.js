<template>
  <div class="lesson-list">
    <h1>Available Lessons</h1>
    <div v-for="lesson in lessons" :key="lesson.id" class="lesson">
      <i :class="lesson.icon" aria-hidden="true"></i>
      <h2>{{ lesson.subject }}</h2>
      <p><strong>Location:</strong> {{ lesson.location }}</p>
      <p><strong>Price:</strong> ${{ lesson.price }}</p>
      <p><strong>Spaces Available:</strong> {{ lesson.spaces }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      lessons: [
        { id: 1, subject: 'Math', location: 'Room 101', price: 50, spaces: 5, icon: 'fa fa-calculator' },
        { id: 2, subject: 'Science', location: 'Room 102', price: 60, spaces: 4, icon: 'fa fa-flask' },
        { id: 3, subject: 'History', location: 'Room 103', price: 55, spaces: 3, icon: 'fa fa-book' },
        { id: 4, subject: 'Art', location: 'Room 104', price: 40, spaces: 2, icon: 'fa fa-paint-brush' },
        { id: 5, subject: 'Music', location: 'Room 105', price: 70, spaces: 1, icon: 'fa fa-music' },
        { id: 6, subject: 'Physics', location: 'Room 106', price: 65, spaces: 5, icon: 'fa fa-atom' },
        { id: 7, subject: 'Chemistry', location: 'Room 107', price: 75, spaces: 4, icon: 'fa fa-flask' },
        { id: 8, subject: 'Biology', location: 'Room 108', price: 80, spaces: 3, icon: 'fa fa-leaf' },
        { id: 9, subject: 'Computer Science', location: 'Room 109', price: 90, spaces: 2, icon: 'fa fa-laptop' },
        { id: 10, subject: 'Physical Education', location: 'Room 110', price: 45, spaces: 1, icon: 'fa fa-futbol' }
      ]
    }
  }
}
</script>

<style scoped>
.lesson-list {
  padding: 20px;
  font-family: Arial, sans-serif;
}

.lesson {
  border: 1px solid #ccc;
  border-radius: 5px;
  padding: 10px;
  margin: 10px 0;
}

.lesson i {
  margin-right: 10px;
  font-size: 24px;
  color: #007BFF;
}
</style>
