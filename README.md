# HL7-JS-Parser
Parse HL7 messages

Example 

```js
const message = `MSH|^~\&|SENDING_APPLICATION|SENDING_FACILITY|RECEIVING_APPLICATION|RECEIVING_FACILITY|20110613072049||ADT^A08|934579920110613072049|P|2.3||||
EVN|A08|20110613072049|||
PID|1||135769||MOUSE^MICKEY^||19281118|M|||123 Main St.^^Lake Buena Vista^FL^32830||(407)939-1289^^^theMainMouse@disney.com|||||1719|99999999||||||||||||||||||||`

const obj = parseHL7(message)

console.log(obj)
```

Output:

```js
​​​​​[
  [
    'MSH',
    ​​​​​​​​​​'|',
    ​​​​​​​​​​'^~&',
    ​​​​​​​​​​'SENDING_APPLICATION',
    ​​​​​​​​​​'SENDING_FACILITY',
    ​​​​​​​​​​'RECEIVING_APPLICATION',
    ​​​​​​​​​​'RECEIVING_FACILITY',
    ​​​​​​​​​​'20110613072049',
    ​​​​​​​​​​'',
    ​​​​​​​​​​[
      'ADT',
      'A08'
    ],
    ​​​​​​​​​​'934579920110613072049',
    ​​​​​​​​​​'P',
    ​​​​​​​​​​'2.3',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​''
  ],
  ​​​​​​​​​​[
    'EVN',
    'A08',
    '20110613072049',
    '',
    '',
    ''
  ],
  ​​​​​​​​​​[
    'PID',
    ​​​​​​​​​​'1',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'135769',
    ​​​​​​​​​​'',
    ​​​​​​​​​​[
      'MOUSE',
      'MICKEY',
      ''
    ],
    ​​​​​​​​​​'',
    ​​​​​​​​​​'19281118',
    ​​​​​​​​​​'M',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​[
      '123 Main St.',
      '',
      'Lake Buena Vista',
      'FL',
      '32830'
    ],
    ​​​​​​​​​​'',
    ​​​​​​​​​​[
      '(407)939-1289',
      '',
      '',
      'theMainMouse@disney.com'
    ],
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'1719',
    ​​​​​​​​​​'99999999',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​'',
    ​​​​​​​​​​''
  ]
]​​​​​
```
