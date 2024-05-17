# Pagination

### Importing

```js
import { CommonPagination } from '@/components/common'
```

### Usage

```html
<CommonPagination />
```

### API

Common props ref：[Common props](https://ant.design/components/pagination#api)

| Parameter                    | Description                                                                                                                                                                                                                                   | Type                                                                                                                                                 | Default                                                                                    |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| theme                        | custom style `Pagination` and `SelectRowPerPage` by [Pagination Design Token](https://ant.design/components/pagination#design-token) <br/>`object` <br/>`{`<br/>`  globalToken: Global Token;`<br/>`componentToken: Component Token;`<br/>`}` | Object                                                                                                                                               | -                                                                                          |
| disabled                     | disable pagination                                                                                                                                                                                                                            | Boolean                                                                                                                                              | -                                                                                          |
| defaultPage                  | uncontrolled current page                                                                                                                                                                                                                     | Number                                                                                                                                               | 1                                                                                          |
| page                         | current page                                                                                                                                                                                                                                  | Number                                                                                                                                               | -                                                                                          |
| total                        | Total number of data items                                                                                                                                                                                                                    | Number                                                                                                                                               | 0                                                                                          |
| defaultRowPerPage            | default items per page                                                                                                                                                                                                                        | Number                                                                                                                                               | 10                                                                                         |
| rowPerPage                   | Number of data items per page                                                                                                                                                                                                                 | Number                                                                                                                                               | 10                                                                                         |
| onChangePage                 | page change callback                                                                                                                                                                                                                          | Function(current, perPage)                                                                                                                           | -                                                                                          |
| showSelectRowPerPage         | Determine whether to show select, it will be true when `rowPerPage` `total > 50`                                                                                                                                                              | Boolean                                                                                                                                              | -                                                                                          |
| totalBoundaryShowSizeChanger | when total larger than it, `showSelectRowPerPage` will be `true`                                                                                                                                                                              | number                                                                                                                                               | 50                                                                                         |
| rowPerPageOptions            | specify the perPageChanger selections                                                                                                                                                                                                         | Array[Number]                                                                                                                                        | [10, 20, 50, 100]                                                                          |
| onChangeRowPerPage           | rowPerPage change callback                                                                                                                                                                                                                    | Function(current, perPage)                                                                                                                           | -                                                                                          |
| hideOnSinglePage             | hide on single page                                                                                                                                                                                                                           | Boolean                                                                                                                                              | false                                                                                      |
| showPrevNextJumpers          | show jump-prev, jump-next                                                                                                                                                                                                                     | Boolean                                                                                                                                              | true                                                                                       |
| showJumperPage               | Determine whether you can jump to pages directly                                                                                                                                                                                              | Boolean / Object                                                                                                                                     | false / {goButton: true}                                                                   |
| showTotal                    | show total records and range                                                                                                                                                                                                                  | Boolean                                                                                                                                              | -                                                                                          |
| totalTemplate                | To customize display the total number and range when showTotal `true`                                                                                                                                                                         | `(total: number, range: [number, number]) => ReactNode \| String`                                                                                    | `` (total: number, range: [number, number]) => `${range[0]} - ${range[1]} จาก ${total}` `` |
| className                    | Specify classname of `Pagination`                                                                                                                                                                                                             | String                                                                                                                                               | -                                                                                          |
| simple                       | Whether to use simple mode                                                                                                                                                                                                                    | Boolean                                                                                                                                              | -                                                                                          |
| locale                       | to set locale text config                                                                                                                                                                                                                     | Object                                                                                                                                               | [th_TH](https://github.com/react-component/pagination/blob/master/src/locale/th_TH.ts)     |
| style                        | Customize inline style of `Pagination`                                                                                                                                                                                                        | Object                                                                                                                                               | -                                                                                          |
| showLessItems                | show less page items                                                                                                                                                                                                                          | Boolean                                                                                                                                              | false                                                                                      |
| showTitle                    | Show page item's title                                                                                                                                                                                                                        | Boolean                                                                                                                                              | true                                                                                       |
| itemRender                   | To customize item's innerHTML                                                                                                                                                                                                                 | Function(current, type: 'page' \| 'prev' \| 'next' \| 'jump-prev' \| 'jump-next', element): React.ReactNode \| `(current, type, element) => element` | -                                                                                          |
| prevIcon                     | Specify the default previous icon                                                                                                                                                                                                             | ReactNode                                                                                                                                            | -                                                                                          |
| nextIcon                     | Specify the default next icon                                                                                                                                                                                                                 | ReactNode                                                                                                                                            | -                                                                                          |
| jumpPrevIcon                 | Specify the default previous icon                                                                                                                                                                                                             | ReactNode                                                                                                                                            | -                                                                                          |
| jumpNextIcon                 | Specify the default next icon                                                                                                                                                                                                                 | ReactNode                                                                                                                                            | -                                                                                          |
| responsive                   | If is not specified, would resize according to the width of the window`size` `Pagination`                                                                                                                                                     | Boolean                                                                                                                                              | -                                                                                          |
| rounded                      | Circular `Pagination` item                                                                                                                                                                                                                    | Boolean                                                                                                                                              | false                                                                                      |
| size                         | Specify the size of , can be set to `Pagination` `small`                                                                                                                                                                                      | default \| small                                                                                                                                     | default                                                                                    |
| style                        | styled `Pagination`                                                                                                                                                                                                                           | `CSSProperties`                                                                                                                                      | -                                                                                          |
| prefixCls                    | Specify Prefix Classname of `Pagination`                                                                                                                                                                                                      | String                                                                                                                                               | -                                                                                          |
| selectPrefixCls              | Specify Prefix Classname of `SelectRowPerPage`                                                                                                                                                                                                | String                                                                                                                                               | -                                                                                          |
| containerStyle               | Customize inline style `Pagination Container`                                                                                                                                                                                                 | React.CSSProperties                                                                                                                                  | -                                                                                          |
| containerClassName           | Specify Classname of `Pagination Container`                                                                                                                                                                                                   | String                                                                                                                                               | -                                                                                          |

### Design Token

https://ant.design/components/pagination#design-token
