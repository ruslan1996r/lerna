`npm i --save-dev lerna`
`npx lerna init`

`npm run diff` - покажет все отличия новой версии от старой
`npm run new-version` - обновит версию приложения. Предварительно надо сделать коммит. Как я понял, эта штука пушит изменения в ветку
помимо этого она выставляет версии обновлений в CHANGELOG.md для каждого проекта, где есть package.json, а также оставляет ссылки на
коммиты в гите, чтобы можно было проследить список изменений в данном коммите

Чтобы всё заработало, надо прописать одинаковые пути в главном package.json и в lerna.json в качестве workspaces ( "packages/*",)