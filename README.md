# Meridian: descargas / downloads

Este repositorio **solo contiene instaladores, notas de versión y los archivos de versión** de Meridian, la aplicación de alarmas para equipos de atención al cliente de **Lumen & Ash**. No hay código fuente aquí.

*This repository only holds installers, release notes and the version files of Meridian, the alarm app for customer-support teams by **Lumen & Ash**. There is no source code here.*

## Descargar / Download

**Última versión / Latest:** [Releases](../../releases/latest)

- Windows 10/11, 64 bits. No hace falta instalar .NET. / Windows 10/11 x64; .NET is bundled.
- Se instala por usuario, sin permisos de administrador. / Installs per user without administrator rights.

### Aviso de SmartScreen / SmartScreen notice

Los instaladores aún no llevan firma digital de Windows, así que SmartScreen puede mostrar «Windows protegió su PC». Pulsa **Más información → Ejecutar de todas formas**. Para estar seguro de que el archivo es el original, compara su SHA-256 con la tabla de abajo.

*The installers are not yet signed with a Windows code-signing certificate, so SmartScreen may show "Windows protected your PC". Choose **More info → Run anyway**. To make sure the file is the original, compare its SHA-256 with the table below.*

En PowerShell / In PowerShell: `Get-FileHash .\Meridian-Setup-<version>.exe -Algorithm SHA256`

## Actualizaciones / Updates

Meridian comprueba `latest.json` de este repositorio al abrirse y cada 12 horas. Solo se descarga ese archivo y su firma: no se envía ningún dato. Cada actualización se verifica con una firma ECDSA P-256 (`latest.json.sig`) y con el SHA-256 del instalador, y **nunca se instala sin que la persona pulse «Actualizar»**. Las versiones `-rc` son pre-releases (`latest-rc.json`) y solo se ofrecen a quien ya tiene una versión `-rc`.

*Meridian reads `latest.json` from this repository when it opens and every 12 hours. Only that file and its signature are downloaded: no data is sent. Every update is verified with an ECDSA P-256 signature (`latest.json.sig`) and the installer's SHA-256, and **it is never installed until the person clicks "Update"**. `-rc` versions are pre-releases (`latest-rc.json`) and are only offered to installations that are already on an `-rc`.*

## SHA-256 de cada versión / SHA-256 of each version

| Versión / Version | Fecha / Date | SHA-256 |
|---|---|---|
| 1.0.0-rc.1 | 2026-11-19 | `a98efd71fb9be9e791f9ec9b807b5502dd9f698a93d2aedc50a833bc73541c41` |
| 1.0.0-rc.2 | 2026-11-19 | `e2963aa3aeb7dbce9327fffe084c86322c80812a87e7f1a9ce27e189fbb2dab2` |
| 1.0.0 | 2026-11-19 | `93b1a6008e81ef6cecf27aaa17c63cc2553c39d3ec0d4315f625e232718f9b80` |
| 1.0.1 | 2026-11-19 | `086f2dfbcf8c6bc1ff36ac4007c819c3db383cd02c93d90a38209e7c8f45aa5f` |
<!-- SHA256-ROWS -->
