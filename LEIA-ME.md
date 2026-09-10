# Cadastro de Materiais — GitHub Pages + Google Drive

O GitHub Pages hospeda somente a interface; registros e fotos ficam na área privada do aplicativo dentro do Google Drive.

## Publicação

1. Crie um repositório no GitHub e envie todos os arquivos desta pasta, inclusive `.github`.
2. Abra **Settings > Pages** e escolha **GitHub Actions** em **Source**.
3. Aguarde a publicação na aba **Actions**. O endereço será parecido com `https://seuusuario.github.io/nome-do-repositorio/`.
4. No Google Cloud Console, abra o cliente OAuth usado pelo aplicativo e adicione `https://seuusuario.github.io` em **Origens JavaScript autorizadas**.
5. Abra o aplicativo e toque em **Conectar com Google**.

O cliente OAuth anterior já está configurado no início de `app.js`. Se usar outro projeto Google, altere somente `clientId`.

## Recursos

- Foto, material e descrição obrigatórios.
- Origem em NC opcional; ao marcar, a referência da NC é obrigatória.
- Responsável opcional.
- Edição, exclusão, busca e filtro por NC.
- Câmera do celular, redução automática da imagem e instalação como PWA.
- Sincronização pelo Google Drive entre celular, tablet e computador.

## Privacidade

O código da interface fica público, mas não contém seus materiais. Os dados usam `appDataFolder`, área privada do Google Drive acessível somente após sua autorização.
