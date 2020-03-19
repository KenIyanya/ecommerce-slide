# app

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).





 <div div class="mt-">
    
    <b-card-group deck >

      <b-card
        border-variant="danger"
        header="Danger"
        header-border-variant="danger"
        header-text-variant="danger"
        align="center"
      >
      <b-card img-src="products.imageLink" img-top>
        </b-card>
       <b-card-text>
        <h5 class="card-title">{{products.name}}</h5>
        <p>{{products.price}}</p>
        <p>{{products.specs}}</p>
        
       </b-card-text>
       <b-button href="#" variant="primary">Add to cat</b-button>
      
        
      </b-card>

    </b-card-group>
  </div>