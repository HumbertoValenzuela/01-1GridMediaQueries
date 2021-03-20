# 01-1GridMediaQueries
Grid ejemplo media queries

```javascript
.servicios {
    display: grid;
    grid-template-columns: 50% 50%;
    grid-template-rows: 50% 50%;
    border: 3px solid black;
    height: 300px;
}
@media screen and (min-width: 768px) {
    .servicios {
    grid-template-columns: 25% 25% 25% 25%;
    grid-template-rows: 33% 33% 33%;
    }
}

/* servicio1 expanda hacia abajo */
.servicio-1 {
    grid-column: 1 / 2;
    grid-row: 1 / 3;
    background-color: darkviolet;
}
/* se expanda hacia abajo */
@media screen and (min-width: 768px) {
    .servicio-1 {
        grid-row: 1 / 4;
    }
}
.servicio-2 {
    background-color: limegreen;
}
@media screen and (min-width: 768px) {
    .servicio-2 {
        grid-column: 2 / 4;
        grid-row: 1 / 4;
    }
    .servicio-3 {
        grid-column: 4 / 5;
        grid-row: 1 / 4;        
    }
}
```
