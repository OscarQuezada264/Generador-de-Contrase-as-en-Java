# Generador-de-Contrase-as-en-Java
Este script en JavaScript genera una contraseña aleatoria de una longitud especificada. Utiliza una combinación de letras, números y caracteres especiales, lo que lo hace útil para aplicaciones que requieren seguridad.
javascript
function generarContrasena(longitud) {
    const caracteres = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*()';
    let contrasena = '';
    for (let i = 0; i < longitud; i++) {
        const indice = Math.floor(Math.random() * caracteres.length);
        contrasena += caracteres[indice];
    }
    return contrasena;
}
