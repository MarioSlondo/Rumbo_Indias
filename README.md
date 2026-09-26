# Rumbo a las Indias

Escena 3D en el navegador: la Pinta, la Niña y la Santa María cruzan el Atlántico hacia poniente en 1492.

**Web:** https://marioslondo.github.io/Rumbo_Indias/

- El sol se calcula para Madrid con la hora real de España: amanece por la popa de la flota y se pone por la proa. También hay un modo de día acelerado.
- Arriba se muestra la fecha de hoy trasladada a 1492 y los días que faltan para llegar a las Indias (12 de octubre).
- **Navegar**: timón con ←/→ o A/D, velas con ↑/↓ o W/S (parado, media vela o a toda vela) y 1/2/3 para elegir la nave.
- **Atacar**: vista aérea con tirachinas (arrastra hacia atrás y suelta). Cada hora en punto aparece el Kraken.
- De noche se encienden los faroles de los barcos. Hay música renacentista, música de batalla y ambiente de mar.

## Probar en local

Hace falta un servidor, porque los módulos no se cargan con `file://`:

```
python3 -m http.server 8000
```

y abre `http://localhost:8000`.

## Contenido

- `index.html`: la página completa (portada, escena, interfaz y shaders).
- `vendor/three/`: Three.js r170 (licencia MIT), incluido para no depender de CDN.
- `audio/`: música, mar, batalla, cañones y kraken, generados con Magnific.

Es un sitio estático: no hace falta compilar nada. En GitHub Pages se publica desde la rama `main`, carpeta `/ (root)`.
