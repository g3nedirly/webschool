<template>
  <div class="container pt-0"> <!-- Mengurangi padding-top di container -->
    <div class="row justify-content-center">
      <div class="col">
        <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
          <!-- Indikator slide -->
          <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3" aria-label="Slide 4"></button>
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="4" aria-label="Slide 5"></button>
          </div>
          
          <!-- Konten gambar carousel -->
          <div class="carousel-inner rounded-5">
            <div class="carousel-item active">
              <img src="@/assets/img/dkv.jpg" class="d-block w-100" alt="..." />
            </div>
            <div class="carousel-item">
              <img src="@/assets/img/juaraa.jpg" class="d-block w-100" alt="..." />
            </div>
            <div class="carousel-item">
              <img src="@/assets/img/srll.jpg" class="d-block w-100" alt="..." />
            </div>
            <div class="carousel-item">
              <img src="@/assets/img/olahraga.jpg" class="d-block w-100" alt="..." />
            </div>
          </div>

          <!-- Tombol navigasi -->
          <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
            <span class="carousel-control-prev-icon rounded-5 bg-secondary" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
            <span class="carousel-control-next-icon rounded-5 bg-secondary" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>
      </div>
    </div>
  </div>

  <!-- Seksi sambutan -->
  <section class="sambutan-container d-flex align-items-center mt-4">
    <div class="sambutan-wrapper p-4 rounded-4 shadow-sm "> <!-- Pembungkus untuk sambutan -->
      <!-- Foto kepala sekolah -->
      <div class="photo-container me-4"> <!-- Memberikan margin di kanan -->
        <img src="@/assets/img/KPLAA.jpeg" alt="Foto Kepala Sekolah" class="photo" />
      </div>
      <!-- Teks sambutan -->
      <div class="text-container">
        <header class="sambutan-header">
          <h2>Sambutan Kepala Sekolah</h2>
          <h3>SMKN 4 Tasikmalaya</h3>
        </header>
        <p>
          Assalamu’alaikum wr.wb. Puji syukur kepada Allah SWT, Tuhan Yang Maha Esa yang telah memberikan rahmat dan anugerah-Nya sehingga website SMKN 4 TASIKMALAYA 
          ini dapat terbit. Salah satu tujuan dari website ini adalah untuk menjawab akan setiap kebutuhan informasi dengan memanfaatkan sarana teknologi informasi yang ada. 
          Kami sadar sepenuhnya dalam rangka memajukan pendidikan di era berkembangnya Teknologi Informasi yang begitu pesat, sangat diperlukan berbagai sarana prasarana yang kondusif, kebutuhan 
          berbagai informasi siswa, guru, orangtua maupun masyarakat, sehingga kami berusaha mewujudkan hal tersebut semaksimal mungkin.
        </p>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Mengurangi padding-top pada container */
.container {
  padding-top: 0; /* Mengurangi jarak atas */
}

/* Mengatur ukuran gambar carousel dengan benar */
.carousel-inner {
  width: 100%;
  height: 70vh; /* Menggunakan 70% dari tinggi layar */
  overflow: hidden; /* Pastikan gambar tidak keluar dari batas */
}

.carousel-inner .carousel-item img {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Pastikan gambar menutupi seluruh area tanpa merubah rasio aspek */
  object-position: center center; /* Gambar akan terpusat di dalam kontainer */
}

/* Styling untuk sambutan */
.sambutan-container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1rem; /* Jarak antara foto dan teks */
}

.sambutan-wrapper {
  display: flex;
  align-items: center;
  gap: 1.5rem; /* Jarak antara foto dan teks di dalam pembungkus */
  background-color: #DEE9EF;
  padding: 1.5rem;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.photo-container {
  flex-shrink: 0;
  width: 200px;
}

.photo-container img {
  width: 100%;
  border-radius: 10px;
  object-fit: cover;
}

.text-container {
  flex-grow: 1;
}

.sambutan-header {
  margin-bottom: 1rem;
}

.sambutan-header h2 {
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
}

.sambutan-header h3 {
  font-size: 1.2rem;
  color: #000000;
  margin-bottom: 1rem;
}
</style>
