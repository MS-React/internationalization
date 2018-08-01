# Directly Training Project

Description:
Directly training app, is an application with **webpack** and **react** to make additions, deletions, and modifications from users.

Application config:

  - By default, the application starts on http://localhost:8080
  - The backend is integrated with the API [MS BE with heroku](https://ms-labs-be.herokuapp.com) you can check the repo here: [MS BE Repository](https://github.com/MS-React/backend)
  - You can point to the local backend with the file **app/constants.js**

  >For now don't commit this **.env.development** or **constants.js** file changes

### Start application

**install packages**
```ssh
npm install
```
**start app**
```ssh
npm start
```
### Dev tools

**run tests**
```ssh
npm test
```

**run test with watch**
```ssh
test:dev
```

**linter rules**
```ssh
npm run lint
```
**sass rules**
```ssh
npm run sass-lint
```

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
