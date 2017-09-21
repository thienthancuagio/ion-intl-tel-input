# ion-intl-tel-input

Ionic library to enter and confirm international telephone numbers. It adds a drop-down flag for any input, user's country discovery, displays a relevant placeholder, and provides formatting / validation methods.


## Installation

This library depends on `BsDropdownModule` from `ngx-bootstrap/dropdown`.
To install this library, run:
```bash
$ npm install ngx-bootstrap --save
```
Then import `BsDropdownModule` at `AppModule`. (more details see : http://valor-software.com/ngx-bootstrap/#/dropdowns)

```typescript
import { BsDropdownModule } from 'ngx-bootstrap/dropdown';

@NgModule({
  ...
  imports: [
      ...
    BsDropdownModule.forRoot()
      ...
  ],
  ...
})
export class AppModule { }
```
## Consuming library

Copy the code into your project:
import file intl-tel-input.css into file your file css

```xml
home-page {
     @import './styles/intl-tel-input';
}

```
You can also import files app.scss

```xml
    @import './styles/intl-tel-input';
```
 
Once library is imported, you can use components in your Ionic application:

```xml

<h1>
  {{phone_number}}
</h1>
<ion-intl-tel-input [(value)]="phoneNumber"></ion-intl-tel-input>
```

### Parameters

| Input | Description |
| ------ | ------ |
| value | Phone number |
