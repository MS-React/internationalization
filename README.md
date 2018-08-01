# Directly Training Project

### install packages
```ssh
npm install
```
### start app
```ssh
npm start
```

### run tests
```ssh
npm test
```

### run linter rules
```ssh
npm run lint
```
### run sass rules
```ssh
npm run sass-lint
```

>For now don't commit this **.env.development** or **constants.js** file changes

# Internationalization - i18n

### Implemented with react-i18nify-lite library

### Translation file: webapp/app/lang/en.js

### Service to handle i18n global in the app: i18nService

**Without parameters:**
```
{i18nService.translate('text.save')}`
```

**With parameters:**
```
{i18nService.translate('text.delete_user', { name: user.name })}
```

**Also you can use components to translate, with your render methods**

**Without parameters:**
```
import { Translate } from 'react-i18nify-lite';

<Translate value="button.save"/>
```
**With parameters:**
```
import { Translate } from 'react-i18nify-lite';

<Translate value="text.delete_user" name={user.name} />
```

You can find more information here [react-i18nify-lite](https://github.com/artisavotins/react-i18nify-lite)


If you need to work with the current **ms-labs-be** app request access to

[Mariano Ravinale](mailto:mravinale@makingsense.com)

[Emanuel Pereyra](mailto:epereyra@makingsense.com)

[Ivan Scoles](mailto:iscoles@makingsense.com)
