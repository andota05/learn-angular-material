# LearnAngularMaterial

## 前提
* ngコマンドが使用できること(使用できる前提で以降記載)

## 初期構築時の流れ
angularプロジェクト作成
```
ng new learn-angular-material
cd learn-angular-material
ng serve
```
Angular Materialスキーマを追加
```
ng add @angular/material

Would you like to proceed? Yes
? Choose a prebuilt theme name, or "custom" for a custom theme: Indigo/Pink        [ Preview: https://material.angular.io?theme=indigo-pink ]
? Set up global Angular Material typography styles? Yes
? Include the Angular animations module? Include and enable animations
```
app.module.tsにコンポーネントをimport
```
// src/app.module.ts
import { MatSlideToggleModule } from '@angular/material/slide-toggle';

...
@NgModule ({
  imports: [
    MatSlideToggleModule,
  ]
})
...
```
app.component.htmlにコンポーネントのタグを追加
```
<mat-slide-toggle>Toggle me!</mat-slide-toggle>
```
