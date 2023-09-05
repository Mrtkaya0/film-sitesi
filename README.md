<body>
    <header>
        <h1>Film Deposu</h1>
        <p>En yeni ve en popüler filmleri burada bulabilirsiniz.</p>
    </header>
    <main>
        <div class="tabs">
            <div class="tab" onclick="showTab('new')">Yeni Filmler</div>
            <div class="tab" onclick="showTab('popular')">En Çok İzlenen Filmler</div>
        </div>
        <div class="content" id="new">
            <h2>Yeni Filmler</h2>
            <p>Bu sekmede en son eklenen filmleri bulabilirsiniz.</p>
            <!-- Yeni filmler listesi buraya gelebilir -->
        </div>
        <div class="content" id="popular" style="display: none;">
            <h2>En Çok İzlenen Filmler</h2>
            <p>Bu sekmede en çok izlenen filmleri bulabilirsiniz.</p>
            <!-- En çok izlenen filmler listesi buraya gelebilir -->
        </div>
    </main>
    <footer>
        <p>&copy; 2023 Film Deposu</p>
        <p>Designed by <a href="#">Adınız Soyadınız</a></p>
    </footer>
    <script>
        function showTab(tabName) {
            var tabs = document.getElementsByClassName("content");
            for (var i = 0; i < tabs.length; i++) {
                tabs[i].style.display = "none";
            }
            document.getElementById(tabName).style.display = "block";
        }
    </script>
</body>
