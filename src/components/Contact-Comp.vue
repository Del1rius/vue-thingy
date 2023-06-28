<template >
     <div class="container-fluid behind">
            <div class="row justify-content-center align-items-center vh-100">
              <div class="col-md-6">
                <div class="card">
                  <div class="card-body">
                    <h2 class="card-title mb-4 text-center fw-bold">Contact Us</h2>
                    <form action="https://formspree.io/f/moqzoggd" method="POST">
                      <div class="mb-3 text-center">
                        <label for="name" class="form-label fs-4 text-white">Name:</label>
                        <input type="text" class="form-control rounded-4" id="name" required>
                      </div>
                      <div class="mb-3 text-center">
                        <label for="email" class="form-label fs-4 text-white">Email:</label>
                        <input type="email" class="form-control rounded-4" id="email" required>
                      </div>
                      <div class="mb-3 text-center">
                        <label for="message" class="form-label fs-4 text-white">Message:</label>
                        <textarea class="form-control rounded-4" id="message" rows="6" required></textarea>
                      </div>
                      <div class="mt-4 mb-4 text-center">
                        <button type="submit" class="btn fs-4">Submit</button>
                    </div>
                    </form>
                  </div>
                </div>
              </div>
            </div>
          </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>

.behind {
    background-color: #BD2C2C;
}

button {
    background-color: #BD2C2C !important;
    color: black !important;
    border: 2px solid white !important;
    border-radius: 20px !important;
    font-weight: bold !important;
}

button:hover {
    background-color: black !important;
    color: #BD2C2C !important;
    border: 2px solid white !important;
    border-radius: 20px !important;
    font-weight: bold !important;
}

.card {
    background-color: gray !important;
}


    
</style>