### Tailwind CSS チートシート

#### 1. レイアウト

- **Display（表示方法）**
  - `block` - `display: block`  
    ブロック要素として表示されます。
    ```html
    <div class="block">Block Element</div>
    ```
  - `inline-block` - `display: inline-block`  
    インラインブロック要素として表示されます。
    ```html
    <div class="inline-block">Inline-Block Element</div>
    ```
  - `inline` - `display: inline`  
    インライン要素として表示されます。
    ```html
    <span class="inline">Inline Element</span>
    ```
  - `flex` - `display: flex`  
    フレックスコンテナとして表示されます。
    ```html
    <div class="flex">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `grid` - `display: grid`  
    グリッドコンテナとして表示されます。
    ```html
    <div class="grid">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```

- **Flexbox（フレックスボックス）**
  - `flex-row` - `flex-direction: row`  
    子要素が横方向に並びます。
    ```html
    <div class="flex flex-row">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `flex-col` - `flex-direction: column`  
    子要素が縦方向に並びます。
    ```html
    <div class="flex flex-col">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `justify-start` - `justify-content: flex-start`  
    子要素が左寄せになります。
    ```html
    <div class="flex justify-start">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `justify-center` - `justify-content: center`  
    子要素が中央寄せになります。
    ```html
    <div class="flex justify-center">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `justify-end` - `justify-content: flex-end`  
    子要素が右寄せになります。
    ```html
    <div class="flex justify-end">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `justify-between` - `justify-content: space-between`  
    子要素の間に等間隔のスペースが入ります。
    ```html
    <div class="flex justify-between">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `items-start` - `align-items: flex-start`  
    子要素が上に揃います。
    ```html
    <div class="flex items-start">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `items-center` - `align-items: center`  
    子要素が中央に揃います。
    ```html
    <div class="flex items-center">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```
  - `items-end` - `align-items: flex-end`  
    子要素が下に揃います。
    ```html
    <div class="flex items-end">
      <div>Item 1</div>
      <div>Item 2</div>
    </div>
    ```

#### 2. スペーシング

- **Margin（マージン）**
  - `m-0` - `margin: 0`
  - `m-1` - `margin: 0.25rem`
  - `m-2` - `margin: 0.5rem`
  - `m-3` - `margin: 0.75rem`
  - `m-4` - `margin: 1rem`
    ```html
    <div class="m-4">Margin 1rem</div>
    ```

- **Padding（パディング）**
  - `p-0` - `padding: 0`
  - `p-1` - `padding: 0.25rem`
  - `p-2` - `padding: 0.5rem`
  - `p-3` - `padding: 0.75rem`
  - `p-4` - `padding: 1rem`
    ```html
    <div class="p-4">Padding 1rem</div>
    ```

- **スペーシングの方向**
  - `mt-2` - `margin-top: 0.5rem`
  - `mr-2` - `margin-right: 0.5rem`
  - `mb-2` - `margin-bottom: 0.5rem`
  - `ml-2` - `margin-left: 0.5rem`
    ```html
    <div class="mt-2 mb-2">Margin Top and Bottom</div>
    ```
  - `pt-2` - `padding-top: 0.5rem`
  - `pr-2` - `padding-right: 0.5rem`
  - `pb-2` - `padding-bottom: 0.5rem`
  - `pl-2` - `padding-left: 0.5rem`
    ```html
    <div class="pt-2 pb-2">Padding Top and Bottom</div>
    ```

#### 3. サイズ

- **Width（幅）**
  - `w-1/2` - `width: 50%`
  - `w-1/3` - `width: 33.333333%`
  - `w-1/4` - `width: 25%`
  - `w-full` - `width: 100%`
    ```html
    <div class="w-1/2">Width 50%</div>
    ```

- **Height（高さ）**
  - `h-1/2` - `height: 50%`
  - `h-1/3` - `height: 33.333333%`
  - `h-1/4` - `height: 25%`
  - `h-full` - `height: 100%`
    ```html
    <div class="h-1/2">Height 50%</div>
    ```

#### 4. 背景色とテキスト色

- **Background Color（背景色）**
  - `bg-white` - `background-color: white`
  - `bg-gray-100` - `background-color: #f7fafc`
  - `bg-blue-500` - `background-color: #4299e1`
    ```html
    <div class="bg-blue-500">Background Blue</div>
    ```

- **Text Color（テキスト色）**
  - `text-white` - `color: white`
  - `text-gray-500` - `color: #a0aec0`
  - `text-blue-500` - `color: #4299e1`
    ```html
    <div class="text-blue-500">Text Blue</div>
    ```

#### 5. ボーダー（境界線）

- **Border Width（ボーダーの幅）**
  - `border` - `border-width: 1px`
  - `border-2` - `border-width: 2px`
  - `border-4` - `border-width: 4px`
    ```html
    <div class="border-2">Border 2px</div>
    ```

- **Border Color（ボーダーの色）**
  - `border-black` - `border-color: black`
  - `border-gray-500` - `border-color: #a0aec0`
  - `border-blue-500` - `border-color: #4299e1`
    ```html
    <div class="border-2 border-blue-500">Border Blue</div>
    ```

- **Border Radius（ボーダーの角の丸み）**
  - `rounded` - `border-radius: 0.25rem`
  - `rounded-full` - `border-radius: 9999px`
  - `rounded-lg` - `border-radius: 0.5rem`
    ```html
    <div class="rounded-lg border">Rounded Border</div>
    ```

#### 6. テキスト

- **Font Size（フォントサイズ）**
  - `text-xs` - `font-size: 0.75rem`
  - `text-sm` - `font-size: 0.875rem`
  - `text-base` - `font-size: 1rem`
  - `text-lg` - `font-size: 1.125rem`
 
 - `text-xl` - `font-size: 1.25rem`
    ```html
    <div class="text-xl">Large Text</div>
    ```

- **Font Weight（フォントの重さ）**
  - `font-light` - `font-weight: 300`
  - `font-normal` - `font-weight: 400`
  - `font-bold` - `font-weight: 700`
    ```html
    <div class="font-bold">Bold Text</div>
    ```

#### 7. その他

- **Shadow（シャドウ）**
  - `shadow` - `box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px 0 rgba(0, 0, 0, 0.06)`
  - `shadow-md` - `box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06)`
  - `shadow-lg` - `box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05)`
    ```html
    <div class="shadow-lg">Large Shadow</div>
    ```

- **Cursor（カーソル）**
  - `cursor-pointer` - `cursor: pointer`
  - `cursor-not-allowed` - `cursor: not-allowed`
    ```html
    <div class="cursor-pointer">Pointer Cursor</div>
    ```

- **Opacity（不透明度）**
  - `opacity-0` - `opacity: 0`
  - `opacity-50` - `opacity: 0.5`
  - `opacity-100` - `opacity: 1`
    ```html
    <div class="opacity-50">50% Opacity</div>
    ```

このチートシートを参考にして、Tailwind CSSを使ったスタイル付けを簡単に行えるようにしてください。必要なクラスをコピペして利用できます。また、Tailwind CSS公式サイトの[ドキュメント](https://tailwindcss.com/docs)も参照すると、より詳細な情報が得られます。