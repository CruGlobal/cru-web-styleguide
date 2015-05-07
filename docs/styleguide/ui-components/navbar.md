---
layout: page
type: page-styleguide-components
title: Navbar
---

Navbars are responsive meta components that serve as navigation headers for your application or site. They begin collapsed (and are toggleable) in mobile views and become horizontal as the available viewport width increases.

Be sure to use a `<nav>` element or, if using a more generic element such as a `<div>`, add a `role="navigation"` to every navbar to explicitly identify it as a landmark region for users of assistive technologies.

## Default

{% example html %}
<nav class="navbar navbar-default">
  <div class="container-fluid">
    <!-- Brand and toggle get grouped for better mobile display -->
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">Brand</a>
    </div>

    <!-- Collect the nav links, forms, and other content for toggling -->
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
      <ul class="nav navbar-nav">
        <li class="active"><a href="#">Link <span class="sr-only">(current)</span></a></li>
        <li><a href="#">Link</a></li>
        <li class="dropdown">
          <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-expanded="false">Dropdown <span class="caret"></span></a>
          <ul class="dropdown-menu" role="menu">
            <li><a href="#">Action</a></li>
            <li><a href="#">Another action</a></li>
            <li><a href="#">Something else here</a></li>
            <li class="divider"></li>
            <li><a href="#">Separated link</a></li>
            <li class="divider"></li>
            <li><a href="#">One more separated link</a></li>
          </ul>
        </li>
      </ul>
      <form class="navbar-form navbar-left" role="search">
        <div class="form-group">
          <input type="text" class="form-control" placeholder="Search">
        </div>
        <button type="submit" class="btn btn-default">Submit</button>
      </form>
      <ul class="nav navbar-nav navbar-right">
        <li><a href="#">Link</a></li>
        <li class="dropdown">
          <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-expanded="false">Dropdown <span class="caret"></span></a>
          <ul class="dropdown-menu" role="menu">
            <li><a href="#">Action</a></li>
            <li><a href="#">Another action</a></li>
            <li><a href="#">Something else here</a></li>
            <li class="divider"></li>
            <li><a href="#">Separated link</a></li>
          </ul>
        </li>
      </ul>
    </div><!-- /.navbar-collapse -->
  </div><!-- /.container-fluid -->
</nav>
{% endexample %}


## Brand Image

Replace the navbar brand with your own image or use an icon as we are doing on cru.org by swapping the text for an `<img>`. Since the `.navbar-brand` has its own height and width, you may need to override some CSS depending on your image.

{% example html %}
    <nav class="navbar navbar-default">
      <div class="container-fluid">
        <div class="navbar-header">
          <a class="navbar-brand" href="#">
            <img alt="Brand" src="data:image/svg+xml;charset=US-ASCII,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22utf-8%22%3F%3E%0A%3C%21--%20Generator%3A%20Adobe%20Illustrator%2017.0.0%2C%20SVG%20Export%20Plug-In%20.%20SVG%20Version%3A%206.00%20Build%200%29%20%20--%3E%0A%3C%21DOCTYPE%20svg%20PUBLIC%20%22-//W3C//DTD%20SVG%201.1//EN%22%20%22http%3A//www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd%22%3E%0A%3Csvg%20version%3D%221.1%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20xmlns%3Axlink%3D%22http%3A//www.w3.org/1999/xlink%22%20x%3D%220px%22%20y%3D%220px%22%0A%09%20width%3D%2270px%22%20height%3D%2249.29px%22%20viewBox%3D%220%200%2075.248%2046.745%22%20enable-background%3D%22new%200%200%2075.248%2046.745%22%20xml%3Aspace%3D%22preserve%22%3E%0A%3Cg%20id%3D%22Master_Logos%22%3E%0A%09%3Cg%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M16.144%2C41.699c-1.892%2C2.15-3.905%2C3.151-6.333%2C3.151c-4.325%2C0-7.844-3.648-7.844-8.132v-0.072%0A%09%09%09c0-4.52%2C3.429-8.06%2C7.808-8.06c2.394%2C0%2C4.387%2C0.937%2C6.273%2C2.949l0.4%2C0.427l1.401-1.307l-0.406-0.429%0A%09%09%09c-1.648-1.748-3.845-3.535-7.632-3.535c-2.665%2C0-5.149%2C1.052-6.994%2C2.963C1.001%2C31.535%2C0%2C34.031%2C0%2C36.682v0.073%0A%09%09%09c0%2C5.509%2C4.385%2C9.991%2C9.775%2C9.991c3.078%2C0%2C5.628-1.234%2C7.796-3.773l0.364-0.427l-1.392-1.301L16.144%2C41.699z%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M23.408%2C30.564v-3.44h-1.932v19.189h1.932v-9.92c0-3.26%2C2.531-7.807%2C6.655-7.807h0.767v-1.89l-0.656-0.005%0A%09%09%09C27.101%2C26.691%2C24.787%2C28.398%2C23.408%2C30.564%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M47.518%2C27.124v10.712c0%2C4.458-2.294%2C7.015-6.295%2C7.015c-4%2C0-6.295-2.557-6.295-7.015V27.124h-1.931%0A%09%09%09v10.784c0%2C5.452%2C3.124%2C8.838%2C8.154%2C8.838h0.144c5.029%2C0%2C8.153-3.386%2C8.153-8.838V27.124H47.518z%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%233DB1C8%22%20points%3D%2262.309%2C0.022%2062.309%2C12.894%2075.248%2C12.894%2075.248%2C14.768%2060.436%2C14.768%2060.436%2C0%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23007398%22%20points%3D%2256.248%2C12.894%2056.248%2C3.836%2058.122%2C3.841%2058.122%2C14.768%2047.042%2C14.768%2047.042%2C12.894%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23DD7D1B%22%20points%3D%2271.426%2C17.074%2071.426%2C18.948%2062.309%2C18.948%2062.309%2C37.109%2060.436%2C37.109%2060.436%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23F9B625%22%20points%3D%2258.123%2C17.074%2058.123%2C26.711%2058.122%2C31.957%2056.248%2C31.957%2056.248%2C18.948%2043.278%2C18.948%20%0A%09%09%0943.278%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M64.966%2C36.329c0-0.454%2C0.366-0.822%2C0.82-0.822c0.454%2C0%2C0.82%2C0.368%2C0.82%2C0.822%0A%09%09%09c0%2C0.451-0.366%2C0.82-0.82%2C0.82C65.332%2C37.149%2C64.966%2C36.781%2C64.966%2C36.329z%20M65.785%2C35.575c-0.414%2C0-0.747%2C0.343-0.747%2C0.755%0A%09%09%09s0.333%2C0.75%2C0.747%2C0.75c0.414%2C0%2C0.747-0.338%2C0.747-0.75S66.199%2C35.575%2C65.785%2C35.575z%20M65.615%2C36.763H65.49v-0.887%0A%09%09%09c0%2C0%2C0.283%2C0%2C0.286%2C0c0.223%2C0%2C0.338%2C0.103%2C0.338%2C0.273c0%2C0.13-0.07%2C0.216-0.175%2C0.256l0.223%2C0.358h-0.145l-0.203-0.328%0A%09%09%09l-0.198%2C0.01V36.763z%20M65.77%2C36.332c0.145-0.003%2C0.218-0.068%2C0.218-0.176c0-0.115-0.073-0.168-0.226-0.168c-0.002%2C0-0.15%2C0-0.15%2C0%0A%09%09%09v0.348L65.77%2C36.332z%22/%3E%0A%09%3C/g%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Layer_4%22%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Labels%22%3E%0A%3C/g%3E%0A%3C/svg%3E%0A">
          </a>
        </div>
      </div>
    </nav>
{% endexample %}


## Forms

Place form content within `.navbar-form` for proper vertical alignment and collapsed behavior in narrow viewports. Use the alignment options to decide where it resides within the navbar content.

As a heads up, `.navbar-form` shares much of its code with `.form-inline` via mixin. Some form controls, like input groups, may require fixed widths to be show up properly within a navbar.

{% example html %}
<nav class="navbar navbar-default">
  <div class="container-fluid">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-2">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img alt="Brand" src="data:image/svg+xml;charset=US-ASCII,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22utf-8%22%3F%3E%0A%3C%21--%20Generator%3A%20Adobe%20Illustrator%2017.0.0%2C%20SVG%20Export%20Plug-In%20.%20SVG%20Version%3A%206.00%20Build%200%29%20%20--%3E%0A%3C%21DOCTYPE%20svg%20PUBLIC%20%22-//W3C//DTD%20SVG%201.1//EN%22%20%22http%3A//www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd%22%3E%0A%3Csvg%20version%3D%221.1%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20xmlns%3Axlink%3D%22http%3A//www.w3.org/1999/xlink%22%20x%3D%220px%22%20y%3D%220px%22%0A%09%20width%3D%2270px%22%20height%3D%2249.29px%22%20viewBox%3D%220%200%2075.248%2046.745%22%20enable-background%3D%22new%200%200%2075.248%2046.745%22%20xml%3Aspace%3D%22preserve%22%3E%0A%3Cg%20id%3D%22Master_Logos%22%3E%0A%09%3Cg%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M16.144%2C41.699c-1.892%2C2.15-3.905%2C3.151-6.333%2C3.151c-4.325%2C0-7.844-3.648-7.844-8.132v-0.072%0A%09%09%09c0-4.52%2C3.429-8.06%2C7.808-8.06c2.394%2C0%2C4.387%2C0.937%2C6.273%2C2.949l0.4%2C0.427l1.401-1.307l-0.406-0.429%0A%09%09%09c-1.648-1.748-3.845-3.535-7.632-3.535c-2.665%2C0-5.149%2C1.052-6.994%2C2.963C1.001%2C31.535%2C0%2C34.031%2C0%2C36.682v0.073%0A%09%09%09c0%2C5.509%2C4.385%2C9.991%2C9.775%2C9.991c3.078%2C0%2C5.628-1.234%2C7.796-3.773l0.364-0.427l-1.392-1.301L16.144%2C41.699z%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M23.408%2C30.564v-3.44h-1.932v19.189h1.932v-9.92c0-3.26%2C2.531-7.807%2C6.655-7.807h0.767v-1.89l-0.656-0.005%0A%09%09%09C27.101%2C26.691%2C24.787%2C28.398%2C23.408%2C30.564%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M47.518%2C27.124v10.712c0%2C4.458-2.294%2C7.015-6.295%2C7.015c-4%2C0-6.295-2.557-6.295-7.015V27.124h-1.931%0A%09%09%09v10.784c0%2C5.452%2C3.124%2C8.838%2C8.154%2C8.838h0.144c5.029%2C0%2C8.153-3.386%2C8.153-8.838V27.124H47.518z%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%233DB1C8%22%20points%3D%2262.309%2C0.022%2062.309%2C12.894%2075.248%2C12.894%2075.248%2C14.768%2060.436%2C14.768%2060.436%2C0%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23007398%22%20points%3D%2256.248%2C12.894%2056.248%2C3.836%2058.122%2C3.841%2058.122%2C14.768%2047.042%2C14.768%2047.042%2C12.894%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23DD7D1B%22%20points%3D%2271.426%2C17.074%2071.426%2C18.948%2062.309%2C18.948%2062.309%2C37.109%2060.436%2C37.109%2060.436%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23F9B625%22%20points%3D%2258.123%2C17.074%2058.123%2C26.711%2058.122%2C31.957%2056.248%2C31.957%2056.248%2C18.948%2043.278%2C18.948%20%0A%09%09%0943.278%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M64.966%2C36.329c0-0.454%2C0.366-0.822%2C0.82-0.822c0.454%2C0%2C0.82%2C0.368%2C0.82%2C0.822%0A%09%09%09c0%2C0.451-0.366%2C0.82-0.82%2C0.82C65.332%2C37.149%2C64.966%2C36.781%2C64.966%2C36.329z%20M65.785%2C35.575c-0.414%2C0-0.747%2C0.343-0.747%2C0.755%0A%09%09%09s0.333%2C0.75%2C0.747%2C0.75c0.414%2C0%2C0.747-0.338%2C0.747-0.75S66.199%2C35.575%2C65.785%2C35.575z%20M65.615%2C36.763H65.49v-0.887%0A%09%09%09c0%2C0%2C0.283%2C0%2C0.286%2C0c0.223%2C0%2C0.338%2C0.103%2C0.338%2C0.273c0%2C0.13-0.07%2C0.216-0.175%2C0.256l0.223%2C0.358h-0.145l-0.203-0.328%0A%09%09%09l-0.198%2C0.01V36.763z%20M65.77%2C36.332c0.145-0.003%2C0.218-0.068%2C0.218-0.176c0-0.115-0.073-0.168-0.226-0.168c-0.002%2C0-0.15%2C0-0.15%2C0%0A%09%09%09v0.348L65.77%2C36.332z%22/%3E%0A%09%3C/g%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Layer_4%22%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Labels%22%3E%0A%3C/g%3E%0A%3C/svg%3E%0A">
      </a>
    </div>
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-2">
      <form class="navbar-form navbar-left" role="search">
        <div class="form-group">
          <input type="text" class="form-control" placeholder="Search">
        </div>
        <button type="submit" class="btn btn-default">Submit</button>
      </form>
    </div>
  </div>
</nav>
{% endexample %}


## Buttons

Add the `.navbar-btn` class to `<button>` elements not residing in a `<form>` to vertically center them in the navbar.

{% example html %}
<nav class="navbar navbar-default">
  <div class="container-fluid">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-3">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img alt="Brand" src="data:image/svg+xml;charset=US-ASCII,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22utf-8%22%3F%3E%0A%3C%21--%20Generator%3A%20Adobe%20Illustrator%2017.0.0%2C%20SVG%20Export%20Plug-In%20.%20SVG%20Version%3A%206.00%20Build%200%29%20%20--%3E%0A%3C%21DOCTYPE%20svg%20PUBLIC%20%22-//W3C//DTD%20SVG%201.1//EN%22%20%22http%3A//www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd%22%3E%0A%3Csvg%20version%3D%221.1%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20xmlns%3Axlink%3D%22http%3A//www.w3.org/1999/xlink%22%20x%3D%220px%22%20y%3D%220px%22%0A%09%20width%3D%2270px%22%20height%3D%2249.29px%22%20viewBox%3D%220%200%2075.248%2046.745%22%20enable-background%3D%22new%200%200%2075.248%2046.745%22%20xml%3Aspace%3D%22preserve%22%3E%0A%3Cg%20id%3D%22Master_Logos%22%3E%0A%09%3Cg%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M16.144%2C41.699c-1.892%2C2.15-3.905%2C3.151-6.333%2C3.151c-4.325%2C0-7.844-3.648-7.844-8.132v-0.072%0A%09%09%09c0-4.52%2C3.429-8.06%2C7.808-8.06c2.394%2C0%2C4.387%2C0.937%2C6.273%2C2.949l0.4%2C0.427l1.401-1.307l-0.406-0.429%0A%09%09%09c-1.648-1.748-3.845-3.535-7.632-3.535c-2.665%2C0-5.149%2C1.052-6.994%2C2.963C1.001%2C31.535%2C0%2C34.031%2C0%2C36.682v0.073%0A%09%09%09c0%2C5.509%2C4.385%2C9.991%2C9.775%2C9.991c3.078%2C0%2C5.628-1.234%2C7.796-3.773l0.364-0.427l-1.392-1.301L16.144%2C41.699z%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M23.408%2C30.564v-3.44h-1.932v19.189h1.932v-9.92c0-3.26%2C2.531-7.807%2C6.655-7.807h0.767v-1.89l-0.656-0.005%0A%09%09%09C27.101%2C26.691%2C24.787%2C28.398%2C23.408%2C30.564%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M47.518%2C27.124v10.712c0%2C4.458-2.294%2C7.015-6.295%2C7.015c-4%2C0-6.295-2.557-6.295-7.015V27.124h-1.931%0A%09%09%09v10.784c0%2C5.452%2C3.124%2C8.838%2C8.154%2C8.838h0.144c5.029%2C0%2C8.153-3.386%2C8.153-8.838V27.124H47.518z%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%233DB1C8%22%20points%3D%2262.309%2C0.022%2062.309%2C12.894%2075.248%2C12.894%2075.248%2C14.768%2060.436%2C14.768%2060.436%2C0%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23007398%22%20points%3D%2256.248%2C12.894%2056.248%2C3.836%2058.122%2C3.841%2058.122%2C14.768%2047.042%2C14.768%2047.042%2C12.894%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23DD7D1B%22%20points%3D%2271.426%2C17.074%2071.426%2C18.948%2062.309%2C18.948%2062.309%2C37.109%2060.436%2C37.109%2060.436%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23F9B625%22%20points%3D%2258.123%2C17.074%2058.123%2C26.711%2058.122%2C31.957%2056.248%2C31.957%2056.248%2C18.948%2043.278%2C18.948%20%0A%09%09%0943.278%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M64.966%2C36.329c0-0.454%2C0.366-0.822%2C0.82-0.822c0.454%2C0%2C0.82%2C0.368%2C0.82%2C0.822%0A%09%09%09c0%2C0.451-0.366%2C0.82-0.82%2C0.82C65.332%2C37.149%2C64.966%2C36.781%2C64.966%2C36.329z%20M65.785%2C35.575c-0.414%2C0-0.747%2C0.343-0.747%2C0.755%0A%09%09%09s0.333%2C0.75%2C0.747%2C0.75c0.414%2C0%2C0.747-0.338%2C0.747-0.75S66.199%2C35.575%2C65.785%2C35.575z%20M65.615%2C36.763H65.49v-0.887%0A%09%09%09c0%2C0%2C0.283%2C0%2C0.286%2C0c0.223%2C0%2C0.338%2C0.103%2C0.338%2C0.273c0%2C0.13-0.07%2C0.216-0.175%2C0.256l0.223%2C0.358h-0.145l-0.203-0.328%0A%09%09%09l-0.198%2C0.01V36.763z%20M65.77%2C36.332c0.145-0.003%2C0.218-0.068%2C0.218-0.176c0-0.115-0.073-0.168-0.226-0.168c-0.002%2C0-0.15%2C0-0.15%2C0%0A%09%09%09v0.348L65.77%2C36.332z%22/%3E%0A%09%3C/g%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Layer_4%22%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Labels%22%3E%0A%3C/g%3E%0A%3C/svg%3E%0A">
      </a>
    </div>
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-3">
      <button type="button" class="btn btn-default navbar-btn">Sign in</button>
    </div>
  </div>
</nav>
{% endexample %}


## Text

Wrap strings of text in an element with `.navbar-text`, usually on a `<p>` tag for proper leading and color.

{% example html %}
<nav class="navbar navbar-default">
  <div class="container-fluid">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-3">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img alt="Brand" src="data:image/svg+xml;charset=US-ASCII,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22utf-8%22%3F%3E%0A%3C%21--%20Generator%3A%20Adobe%20Illustrator%2017.0.0%2C%20SVG%20Export%20Plug-In%20.%20SVG%20Version%3A%206.00%20Build%200%29%20%20--%3E%0A%3C%21DOCTYPE%20svg%20PUBLIC%20%22-//W3C//DTD%20SVG%201.1//EN%22%20%22http%3A//www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd%22%3E%0A%3Csvg%20version%3D%221.1%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20xmlns%3Axlink%3D%22http%3A//www.w3.org/1999/xlink%22%20x%3D%220px%22%20y%3D%220px%22%0A%09%20width%3D%2270px%22%20height%3D%2249.29px%22%20viewBox%3D%220%200%2075.248%2046.745%22%20enable-background%3D%22new%200%200%2075.248%2046.745%22%20xml%3Aspace%3D%22preserve%22%3E%0A%3Cg%20id%3D%22Master_Logos%22%3E%0A%09%3Cg%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M16.144%2C41.699c-1.892%2C2.15-3.905%2C3.151-6.333%2C3.151c-4.325%2C0-7.844-3.648-7.844-8.132v-0.072%0A%09%09%09c0-4.52%2C3.429-8.06%2C7.808-8.06c2.394%2C0%2C4.387%2C0.937%2C6.273%2C2.949l0.4%2C0.427l1.401-1.307l-0.406-0.429%0A%09%09%09c-1.648-1.748-3.845-3.535-7.632-3.535c-2.665%2C0-5.149%2C1.052-6.994%2C2.963C1.001%2C31.535%2C0%2C34.031%2C0%2C36.682v0.073%0A%09%09%09c0%2C5.509%2C4.385%2C9.991%2C9.775%2C9.991c3.078%2C0%2C5.628-1.234%2C7.796-3.773l0.364-0.427l-1.392-1.301L16.144%2C41.699z%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M23.408%2C30.564v-3.44h-1.932v19.189h1.932v-9.92c0-3.26%2C2.531-7.807%2C6.655-7.807h0.767v-1.89l-0.656-0.005%0A%09%09%09C27.101%2C26.691%2C24.787%2C28.398%2C23.408%2C30.564%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M47.518%2C27.124v10.712c0%2C4.458-2.294%2C7.015-6.295%2C7.015c-4%2C0-6.295-2.557-6.295-7.015V27.124h-1.931%0A%09%09%09v10.784c0%2C5.452%2C3.124%2C8.838%2C8.154%2C8.838h0.144c5.029%2C0%2C8.153-3.386%2C8.153-8.838V27.124H47.518z%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%233DB1C8%22%20points%3D%2262.309%2C0.022%2062.309%2C12.894%2075.248%2C12.894%2075.248%2C14.768%2060.436%2C14.768%2060.436%2C0%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23007398%22%20points%3D%2256.248%2C12.894%2056.248%2C3.836%2058.122%2C3.841%2058.122%2C14.768%2047.042%2C14.768%2047.042%2C12.894%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23DD7D1B%22%20points%3D%2271.426%2C17.074%2071.426%2C18.948%2062.309%2C18.948%2062.309%2C37.109%2060.436%2C37.109%2060.436%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23F9B625%22%20points%3D%2258.123%2C17.074%2058.123%2C26.711%2058.122%2C31.957%2056.248%2C31.957%2056.248%2C18.948%2043.278%2C18.948%20%0A%09%09%0943.278%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M64.966%2C36.329c0-0.454%2C0.366-0.822%2C0.82-0.822c0.454%2C0%2C0.82%2C0.368%2C0.82%2C0.822%0A%09%09%09c0%2C0.451-0.366%2C0.82-0.82%2C0.82C65.332%2C37.149%2C64.966%2C36.781%2C64.966%2C36.329z%20M65.785%2C35.575c-0.414%2C0-0.747%2C0.343-0.747%2C0.755%0A%09%09%09s0.333%2C0.75%2C0.747%2C0.75c0.414%2C0%2C0.747-0.338%2C0.747-0.75S66.199%2C35.575%2C65.785%2C35.575z%20M65.615%2C36.763H65.49v-0.887%0A%09%09%09c0%2C0%2C0.283%2C0%2C0.286%2C0c0.223%2C0%2C0.338%2C0.103%2C0.338%2C0.273c0%2C0.13-0.07%2C0.216-0.175%2C0.256l0.223%2C0.358h-0.145l-0.203-0.328%0A%09%09%09l-0.198%2C0.01V36.763z%20M65.77%2C36.332c0.145-0.003%2C0.218-0.068%2C0.218-0.176c0-0.115-0.073-0.168-0.226-0.168c-0.002%2C0-0.15%2C0-0.15%2C0%0A%09%09%09v0.348L65.77%2C36.332z%22/%3E%0A%09%3C/g%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Layer_4%22%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Labels%22%3E%0A%3C/g%3E%0A%3C/svg%3E%0A">
      </a>
    </div>
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-3">
        <p class="navbar-text">Signed in as Jimmy Dempsey</p>
    </div>
  </div>
</nav>
{% endexample %}


## Non-nav links

For folks using standard links that are not within the regular navbar navigation component, use the `.navbar-link` class to add the proper colors.

{% example html %}
<nav class="navbar navbar-default">
  <div class="container-fluid">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-3">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img alt="Brand" src="data:image/svg+xml;charset=US-ASCII,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22utf-8%22%3F%3E%0A%3C%21--%20Generator%3A%20Adobe%20Illustrator%2017.0.0%2C%20SVG%20Export%20Plug-In%20.%20SVG%20Version%3A%206.00%20Build%200%29%20%20--%3E%0A%3C%21DOCTYPE%20svg%20PUBLIC%20%22-//W3C//DTD%20SVG%201.1//EN%22%20%22http%3A//www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd%22%3E%0A%3Csvg%20version%3D%221.1%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20xmlns%3Axlink%3D%22http%3A//www.w3.org/1999/xlink%22%20x%3D%220px%22%20y%3D%220px%22%0A%09%20width%3D%2270px%22%20height%3D%2249.29px%22%20viewBox%3D%220%200%2075.248%2046.745%22%20enable-background%3D%22new%200%200%2075.248%2046.745%22%20xml%3Aspace%3D%22preserve%22%3E%0A%3Cg%20id%3D%22Master_Logos%22%3E%0A%09%3Cg%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M16.144%2C41.699c-1.892%2C2.15-3.905%2C3.151-6.333%2C3.151c-4.325%2C0-7.844-3.648-7.844-8.132v-0.072%0A%09%09%09c0-4.52%2C3.429-8.06%2C7.808-8.06c2.394%2C0%2C4.387%2C0.937%2C6.273%2C2.949l0.4%2C0.427l1.401-1.307l-0.406-0.429%0A%09%09%09c-1.648-1.748-3.845-3.535-7.632-3.535c-2.665%2C0-5.149%2C1.052-6.994%2C2.963C1.001%2C31.535%2C0%2C34.031%2C0%2C36.682v0.073%0A%09%09%09c0%2C5.509%2C4.385%2C9.991%2C9.775%2C9.991c3.078%2C0%2C5.628-1.234%2C7.796-3.773l0.364-0.427l-1.392-1.301L16.144%2C41.699z%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M23.408%2C30.564v-3.44h-1.932v19.189h1.932v-9.92c0-3.26%2C2.531-7.807%2C6.655-7.807h0.767v-1.89l-0.656-0.005%0A%09%09%09C27.101%2C26.691%2C24.787%2C28.398%2C23.408%2C30.564%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M47.518%2C27.124v10.712c0%2C4.458-2.294%2C7.015-6.295%2C7.015c-4%2C0-6.295-2.557-6.295-7.015V27.124h-1.931%0A%09%09%09v10.784c0%2C5.452%2C3.124%2C8.838%2C8.154%2C8.838h0.144c5.029%2C0%2C8.153-3.386%2C8.153-8.838V27.124H47.518z%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%233DB1C8%22%20points%3D%2262.309%2C0.022%2062.309%2C12.894%2075.248%2C12.894%2075.248%2C14.768%2060.436%2C14.768%2060.436%2C0%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23007398%22%20points%3D%2256.248%2C12.894%2056.248%2C3.836%2058.122%2C3.841%2058.122%2C14.768%2047.042%2C14.768%2047.042%2C12.894%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23DD7D1B%22%20points%3D%2271.426%2C17.074%2071.426%2C18.948%2062.309%2C18.948%2062.309%2C37.109%2060.436%2C37.109%2060.436%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23F9B625%22%20points%3D%2258.123%2C17.074%2058.123%2C26.711%2058.122%2C31.957%2056.248%2C31.957%2056.248%2C18.948%2043.278%2C18.948%20%0A%09%09%0943.278%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M64.966%2C36.329c0-0.454%2C0.366-0.822%2C0.82-0.822c0.454%2C0%2C0.82%2C0.368%2C0.82%2C0.822%0A%09%09%09c0%2C0.451-0.366%2C0.82-0.82%2C0.82C65.332%2C37.149%2C64.966%2C36.781%2C64.966%2C36.329z%20M65.785%2C35.575c-0.414%2C0-0.747%2C0.343-0.747%2C0.755%0A%09%09%09s0.333%2C0.75%2C0.747%2C0.75c0.414%2C0%2C0.747-0.338%2C0.747-0.75S66.199%2C35.575%2C65.785%2C35.575z%20M65.615%2C36.763H65.49v-0.887%0A%09%09%09c0%2C0%2C0.283%2C0%2C0.286%2C0c0.223%2C0%2C0.338%2C0.103%2C0.338%2C0.273c0%2C0.13-0.07%2C0.216-0.175%2C0.256l0.223%2C0.358h-0.145l-0.203-0.328%0A%09%09%09l-0.198%2C0.01V36.763z%20M65.77%2C36.332c0.145-0.003%2C0.218-0.068%2C0.218-0.176c0-0.115-0.073-0.168-0.226-0.168c-0.002%2C0-0.15%2C0-0.15%2C0%0A%09%09%09v0.348L65.77%2C36.332z%22/%3E%0A%09%3C/g%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Layer_4%22%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Labels%22%3E%0A%3C/g%3E%0A%3C/svg%3E%0A">
      </a>
    </div>
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-3">
    <p class="navbar-text navbar-right">Signed in as <a href="#" class="navbar-link">Jimmy Dempsey</a></p>
    </div>
  </div>
</nav>
{% endexample %}


## Component Alignment

Align nav links, forms, buttons, or text, using the `.navbar-left` or `.navbar-right` utility classes. Both classes will add a CSS float in the specified direction. For example, to align nav links, put them in a separate `<ul>` with the respective utility class applied.

These classes are mixin-ed versions of `.u-floatLeft` and `.u-floatRight`, but they're scoped to media queries for easier handling of navbar components across device sizes.


## Fixed to top

Add `.navbar-fixed-top` and include a `.container` or `.container-fluid` to center and give some padding to the navbar content.

{% example html %}
<nav class="navbar  navbar-default  navbar-fixed-top">
  <div class="container-fluid">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-3">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img alt="Brand" src="data:image/svg+xml;charset=US-ASCII,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22utf-8%22%3F%3E%0A%3C%21--%20Generator%3A%20Adobe%20Illustrator%2017.0.0%2C%20SVG%20Export%20Plug-In%20.%20SVG%20Version%3A%206.00%20Build%200%29%20%20--%3E%0A%3C%21DOCTYPE%20svg%20PUBLIC%20%22-//W3C//DTD%20SVG%201.1//EN%22%20%22http%3A//www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd%22%3E%0A%3Csvg%20version%3D%221.1%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20xmlns%3Axlink%3D%22http%3A//www.w3.org/1999/xlink%22%20x%3D%220px%22%20y%3D%220px%22%0A%09%20width%3D%2270px%22%20height%3D%2249.29px%22%20viewBox%3D%220%200%2075.248%2046.745%22%20enable-background%3D%22new%200%200%2075.248%2046.745%22%20xml%3Aspace%3D%22preserve%22%3E%0A%3Cg%20id%3D%22Master_Logos%22%3E%0A%09%3Cg%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M16.144%2C41.699c-1.892%2C2.15-3.905%2C3.151-6.333%2C3.151c-4.325%2C0-7.844-3.648-7.844-8.132v-0.072%0A%09%09%09c0-4.52%2C3.429-8.06%2C7.808-8.06c2.394%2C0%2C4.387%2C0.937%2C6.273%2C2.949l0.4%2C0.427l1.401-1.307l-0.406-0.429%0A%09%09%09c-1.648-1.748-3.845-3.535-7.632-3.535c-2.665%2C0-5.149%2C1.052-6.994%2C2.963C1.001%2C31.535%2C0%2C34.031%2C0%2C36.682v0.073%0A%09%09%09c0%2C5.509%2C4.385%2C9.991%2C9.775%2C9.991c3.078%2C0%2C5.628-1.234%2C7.796-3.773l0.364-0.427l-1.392-1.301L16.144%2C41.699z%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M23.408%2C30.564v-3.44h-1.932v19.189h1.932v-9.92c0-3.26%2C2.531-7.807%2C6.655-7.807h0.767v-1.89l-0.656-0.005%0A%09%09%09C27.101%2C26.691%2C24.787%2C28.398%2C23.408%2C30.564%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M47.518%2C27.124v10.712c0%2C4.458-2.294%2C7.015-6.295%2C7.015c-4%2C0-6.295-2.557-6.295-7.015V27.124h-1.931%0A%09%09%09v10.784c0%2C5.452%2C3.124%2C8.838%2C8.154%2C8.838h0.144c5.029%2C0%2C8.153-3.386%2C8.153-8.838V27.124H47.518z%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%233DB1C8%22%20points%3D%2262.309%2C0.022%2062.309%2C12.894%2075.248%2C12.894%2075.248%2C14.768%2060.436%2C14.768%2060.436%2C0%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23007398%22%20points%3D%2256.248%2C12.894%2056.248%2C3.836%2058.122%2C3.841%2058.122%2C14.768%2047.042%2C14.768%2047.042%2C12.894%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23DD7D1B%22%20points%3D%2271.426%2C17.074%2071.426%2C18.948%2062.309%2C18.948%2062.309%2C37.109%2060.436%2C37.109%2060.436%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23F9B625%22%20points%3D%2258.123%2C17.074%2058.123%2C26.711%2058.122%2C31.957%2056.248%2C31.957%2056.248%2C18.948%2043.278%2C18.948%20%0A%09%09%0943.278%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M64.966%2C36.329c0-0.454%2C0.366-0.822%2C0.82-0.822c0.454%2C0%2C0.82%2C0.368%2C0.82%2C0.822%0A%09%09%09c0%2C0.451-0.366%2C0.82-0.82%2C0.82C65.332%2C37.149%2C64.966%2C36.781%2C64.966%2C36.329z%20M65.785%2C35.575c-0.414%2C0-0.747%2C0.343-0.747%2C0.755%0A%09%09%09s0.333%2C0.75%2C0.747%2C0.75c0.414%2C0%2C0.747-0.338%2C0.747-0.75S66.199%2C35.575%2C65.785%2C35.575z%20M65.615%2C36.763H65.49v-0.887%0A%09%09%09c0%2C0%2C0.283%2C0%2C0.286%2C0c0.223%2C0%2C0.338%2C0.103%2C0.338%2C0.273c0%2C0.13-0.07%2C0.216-0.175%2C0.256l0.223%2C0.358h-0.145l-0.203-0.328%0A%09%09%09l-0.198%2C0.01V36.763z%20M65.77%2C36.332c0.145-0.003%2C0.218-0.068%2C0.218-0.176c0-0.115-0.073-0.168-0.226-0.168c-0.002%2C0-0.15%2C0-0.15%2C0%0A%09%09%09v0.348L65.77%2C36.332z%22/%3E%0A%09%3C/g%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Layer_4%22%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Labels%22%3E%0A%3C/g%3E%0A%3C/svg%3E%0A">
      </a>
    </div>
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-3">
    </div>
  </div>
</nav>
{% endexample %}

The fixed navbar will overlay your other content, unless you add padding to the top of the `<body>`.

## Fixed to bottom

{% example html %}
<nav class="navbar  navbar-default  fixed-to-bottom">
  <div class="container-fluid">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-3">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img alt="Brand" src="data:image/svg+xml;charset=US-ASCII,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22utf-8%22%3F%3E%0A%3C%21--%20Generator%3A%20Adobe%20Illustrator%2017.0.0%2C%20SVG%20Export%20Plug-In%20.%20SVG%20Version%3A%206.00%20Build%200%29%20%20--%3E%0A%3C%21DOCTYPE%20svg%20PUBLIC%20%22-//W3C//DTD%20SVG%201.1//EN%22%20%22http%3A//www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd%22%3E%0A%3Csvg%20version%3D%221.1%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20xmlns%3Axlink%3D%22http%3A//www.w3.org/1999/xlink%22%20x%3D%220px%22%20y%3D%220px%22%0A%09%20width%3D%2270px%22%20height%3D%2249.29px%22%20viewBox%3D%220%200%2075.248%2046.745%22%20enable-background%3D%22new%200%200%2075.248%2046.745%22%20xml%3Aspace%3D%22preserve%22%3E%0A%3Cg%20id%3D%22Master_Logos%22%3E%0A%09%3Cg%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M16.144%2C41.699c-1.892%2C2.15-3.905%2C3.151-6.333%2C3.151c-4.325%2C0-7.844-3.648-7.844-8.132v-0.072%0A%09%09%09c0-4.52%2C3.429-8.06%2C7.808-8.06c2.394%2C0%2C4.387%2C0.937%2C6.273%2C2.949l0.4%2C0.427l1.401-1.307l-0.406-0.429%0A%09%09%09c-1.648-1.748-3.845-3.535-7.632-3.535c-2.665%2C0-5.149%2C1.052-6.994%2C2.963C1.001%2C31.535%2C0%2C34.031%2C0%2C36.682v0.073%0A%09%09%09c0%2C5.509%2C4.385%2C9.991%2C9.775%2C9.991c3.078%2C0%2C5.628-1.234%2C7.796-3.773l0.364-0.427l-1.392-1.301L16.144%2C41.699z%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M23.408%2C30.564v-3.44h-1.932v19.189h1.932v-9.92c0-3.26%2C2.531-7.807%2C6.655-7.807h0.767v-1.89l-0.656-0.005%0A%09%09%09C27.101%2C26.691%2C24.787%2C28.398%2C23.408%2C30.564%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M47.518%2C27.124v10.712c0%2C4.458-2.294%2C7.015-6.295%2C7.015c-4%2C0-6.295-2.557-6.295-7.015V27.124h-1.931%0A%09%09%09v10.784c0%2C5.452%2C3.124%2C8.838%2C8.154%2C8.838h0.144c5.029%2C0%2C8.153-3.386%2C8.153-8.838V27.124H47.518z%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%233DB1C8%22%20points%3D%2262.309%2C0.022%2062.309%2C12.894%2075.248%2C12.894%2075.248%2C14.768%2060.436%2C14.768%2060.436%2C0%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23007398%22%20points%3D%2256.248%2C12.894%2056.248%2C3.836%2058.122%2C3.841%2058.122%2C14.768%2047.042%2C14.768%2047.042%2C12.894%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23DD7D1B%22%20points%3D%2271.426%2C17.074%2071.426%2C18.948%2062.309%2C18.948%2062.309%2C37.109%2060.436%2C37.109%2060.436%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23F9B625%22%20points%3D%2258.123%2C17.074%2058.123%2C26.711%2058.122%2C31.957%2056.248%2C31.957%2056.248%2C18.948%2043.278%2C18.948%20%0A%09%09%0943.278%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M64.966%2C36.329c0-0.454%2C0.366-0.822%2C0.82-0.822c0.454%2C0%2C0.82%2C0.368%2C0.82%2C0.822%0A%09%09%09c0%2C0.451-0.366%2C0.82-0.82%2C0.82C65.332%2C37.149%2C64.966%2C36.781%2C64.966%2C36.329z%20M65.785%2C35.575c-0.414%2C0-0.747%2C0.343-0.747%2C0.755%0A%09%09%09s0.333%2C0.75%2C0.747%2C0.75c0.414%2C0%2C0.747-0.338%2C0.747-0.75S66.199%2C35.575%2C65.785%2C35.575z%20M65.615%2C36.763H65.49v-0.887%0A%09%09%09c0%2C0%2C0.283%2C0%2C0.286%2C0c0.223%2C0%2C0.338%2C0.103%2C0.338%2C0.273c0%2C0.13-0.07%2C0.216-0.175%2C0.256l0.223%2C0.358h-0.145l-0.203-0.328%0A%09%09%09l-0.198%2C0.01V36.763z%20M65.77%2C36.332c0.145-0.003%2C0.218-0.068%2C0.218-0.176c0-0.115-0.073-0.168-0.226-0.168c-0.002%2C0-0.15%2C0-0.15%2C0%0A%09%09%09v0.348L65.77%2C36.332z%22/%3E%0A%09%3C/g%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Layer_4%22%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Labels%22%3E%0A%3C/g%3E%0A%3C/svg%3E%0A">
      </a>
    </div>
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-3">
    </div>
  </div>
</nav>
{% endexample %}

The fixed navbar will overlay your other content, unless you add padding to the bottom of the `<body>`.


## Static top

Create a full-width navbar that scrolls away with the page by adding `.navbar-static-top` and include a `.container` or `.container-fluid` to center and add some padding to the navbar content.

Unlike the `.navbar-fixed-*` classes, you do not need to change any padding on the body.

{% example html %}
<nav class="navbar  navbar-default  navbar-static-top">
  <div class="container-fluid">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-3">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img alt="Brand" src="data:image/svg+xml;charset=US-ASCII,%3C%3Fxml%20version%3D%221.0%22%20encoding%3D%22utf-8%22%3F%3E%0A%3C%21--%20Generator%3A%20Adobe%20Illustrator%2017.0.0%2C%20SVG%20Export%20Plug-In%20.%20SVG%20Version%3A%206.00%20Build%200%29%20%20--%3E%0A%3C%21DOCTYPE%20svg%20PUBLIC%20%22-//W3C//DTD%20SVG%201.1//EN%22%20%22http%3A//www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd%22%3E%0A%3Csvg%20version%3D%221.1%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20xmlns%3Axlink%3D%22http%3A//www.w3.org/1999/xlink%22%20x%3D%220px%22%20y%3D%220px%22%0A%09%20width%3D%2270px%22%20height%3D%2249.29px%22%20viewBox%3D%220%200%2075.248%2046.745%22%20enable-background%3D%22new%200%200%2075.248%2046.745%22%20xml%3Aspace%3D%22preserve%22%3E%0A%3Cg%20id%3D%22Master_Logos%22%3E%0A%09%3Cg%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M16.144%2C41.699c-1.892%2C2.15-3.905%2C3.151-6.333%2C3.151c-4.325%2C0-7.844-3.648-7.844-8.132v-0.072%0A%09%09%09c0-4.52%2C3.429-8.06%2C7.808-8.06c2.394%2C0%2C4.387%2C0.937%2C6.273%2C2.949l0.4%2C0.427l1.401-1.307l-0.406-0.429%0A%09%09%09c-1.648-1.748-3.845-3.535-7.632-3.535c-2.665%2C0-5.149%2C1.052-6.994%2C2.963C1.001%2C31.535%2C0%2C34.031%2C0%2C36.682v0.073%0A%09%09%09c0%2C5.509%2C4.385%2C9.991%2C9.775%2C9.991c3.078%2C0%2C5.628-1.234%2C7.796-3.773l0.364-0.427l-1.392-1.301L16.144%2C41.699z%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M23.408%2C30.564v-3.44h-1.932v19.189h1.932v-9.92c0-3.26%2C2.531-7.807%2C6.655-7.807h0.767v-1.89l-0.656-0.005%0A%09%09%09C27.101%2C26.691%2C24.787%2C28.398%2C23.408%2C30.564%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M47.518%2C27.124v10.712c0%2C4.458-2.294%2C7.015-6.295%2C7.015c-4%2C0-6.295-2.557-6.295-7.015V27.124h-1.931%0A%09%09%09v10.784c0%2C5.452%2C3.124%2C8.838%2C8.154%2C8.838h0.144c5.029%2C0%2C8.153-3.386%2C8.153-8.838V27.124H47.518z%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%233DB1C8%22%20points%3D%2262.309%2C0.022%2062.309%2C12.894%2075.248%2C12.894%2075.248%2C14.768%2060.436%2C14.768%2060.436%2C0%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23007398%22%20points%3D%2256.248%2C12.894%2056.248%2C3.836%2058.122%2C3.841%2058.122%2C14.768%2047.042%2C14.768%2047.042%2C12.894%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23DD7D1B%22%20points%3D%2271.426%2C17.074%2071.426%2C18.948%2062.309%2C18.948%2062.309%2C37.109%2060.436%2C37.109%2060.436%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpolygon%20fill%3D%22%23F9B625%22%20points%3D%2258.123%2C17.074%2058.123%2C26.711%2058.122%2C31.957%2056.248%2C31.957%2056.248%2C18.948%2043.278%2C18.948%20%0A%09%09%0943.278%2C17.074%20%09%09%22/%3E%0A%09%09%3Cpath%20fill%3D%22%23626062%22%20d%3D%22M64.966%2C36.329c0-0.454%2C0.366-0.822%2C0.82-0.822c0.454%2C0%2C0.82%2C0.368%2C0.82%2C0.822%0A%09%09%09c0%2C0.451-0.366%2C0.82-0.82%2C0.82C65.332%2C37.149%2C64.966%2C36.781%2C64.966%2C36.329z%20M65.785%2C35.575c-0.414%2C0-0.747%2C0.343-0.747%2C0.755%0A%09%09%09s0.333%2C0.75%2C0.747%2C0.75c0.414%2C0%2C0.747-0.338%2C0.747-0.75S66.199%2C35.575%2C65.785%2C35.575z%20M65.615%2C36.763H65.49v-0.887%0A%09%09%09c0%2C0%2C0.283%2C0%2C0.286%2C0c0.223%2C0%2C0.338%2C0.103%2C0.338%2C0.273c0%2C0.13-0.07%2C0.216-0.175%2C0.256l0.223%2C0.358h-0.145l-0.203-0.328%0A%09%09%09l-0.198%2C0.01V36.763z%20M65.77%2C36.332c0.145-0.003%2C0.218-0.068%2C0.218-0.176c0-0.115-0.073-0.168-0.226-0.168c-0.002%2C0-0.15%2C0-0.15%2C0%0A%09%09%09v0.348L65.77%2C36.332z%22/%3E%0A%09%3C/g%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Layer_4%22%3E%0A%3C/g%3E%0A%3Cg%20id%3D%22Labels%22%3E%0A%3C/g%3E%0A%3C/svg%3E%0A">
      </a>
    </div>
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-3">
    </div>
  </div>
</nav>
{% endexample %}
