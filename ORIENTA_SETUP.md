# Orienta Triana — configuración segura

Este módulo se encuentra en `orienta.html` y utiliza datos ficticios hasta completar la configuración.

## Firebase

1. Activar Firestore en el proyecto `sistema-academico-sanpedro`.
2. Activar Authentication mediante correo y contraseña.
3. Crear únicamente la cuenta personal del orientador.
4. Publicar las reglas incluidas en `firestore.rules`.
5. Probar primero con códigos ficticios.
6. No introducir nombres hasta verificar el cifrado de la bóveda.

## Modelo previsto

Todos los documentos de Orientación quedarán bajo:

```
users/{uid}/students/{studentId}
users/{uid}/enrollments/{enrollmentId}
users/{uid}/interviews/{interviewId}
users/{uid}/actions/{actionId}
users/{uid}/tasks/{taskId}
users/{uid}/decisions/{decisionId}
users/{uid}/identityVault/{studentId}
```

El identificador permanente `A001` se comparte conceptualmente con Atención a la Diversidad. La bóveda código–nombre se cifra en el navegador antes de escribir en Firestore.

## Estado

La página actual es una base navegable. Todavía no guarda alumnado real ni nombres en Firebase.
