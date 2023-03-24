<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
    <div class="container-fluid">
        <a href="/" class="navbar-brand">Probabilidad</a>
        <button
            type="button"
            class="navbar-toggler"
            data-bs-toggle="collapse"
            data-bs-target="navbarCollapse"
        >
            <span class="navbar-toggler-icon" />
        </button>
        <div class="collapse navbar-collapse" id="navbarCollapse">
            <div class="navbar-nav">
                <a href="/about" class="nav-item nav-link active">About</a>
                <a href="/grafico" class="nav-item nav-link">Gráfico</a>
                <a href="/funcion" class="nav-item nav-link">Función</a>
                <a
                    class="nav-link dropdown-toggle"
                    href="/"
                    id="navbarDropdown"
                    role="button"
                    data-bs-toggle="dropdown"
                    aria-expanded="false"
                >
                    Dropdown
                </a>
                <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                    <li>
                        <a class="dropdown-item" href="/grafico">Gráfico</a>
                    </li>
                    <li>
                        <a class="dropdown-item" href="/about">About</a>
                    </li>
                    <li><hr class="dropdown-divider" /></li>
                    <li>
                        <a class="dropdown-item" href="/about">About</a>
                    </li>
                </ul>
                <a href="/about" class="nav-item nav-link ms-auto">Salir</a>
            </div>
        </div>
    </div>
</nav>

<slot />
