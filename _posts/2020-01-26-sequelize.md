---
# 3 :: 파일 이름 2019-12-05-XXXXXXX  
layout: post # 양식 
title: Sequelize # 1 :: 글제목
tags: [Node.js]  # 분류
---

### Sequeilze
```
npm install sequelize
```

```js
sequelize.define(modelName, attribute, options);

const user = sequelize.define('user', {
    // atribute
    colume1 : {
        field : "fieldName",
        type : DataTypes.UUID, // STRING, INTEGER, ...
        defaultValue : DataTypes.UUIDV4,
        primaryKey : true,
        allowNull : true,
        unique : true,
        
    }
}, {
    // options
    
    timestamps : true,
    // updatedAt, createdAt 컬럼을 추가해줌.
    
    paranoid : true,
    // deletedAt 컬럼을 추가해줌. 해당 row 삭제시 실제 데이터베이스에서 삭제되지 않고,
    // deletedAt 컬럼 값만 갱신함.
    // 조회시 deletedAt 이 null 이 아닐 경우 가져오지 않음.

    underscored : true,
    // default : camelCase , DB 컬럼 이름을 var_id 와 같은 언더스코어를 사용
    
    freezeTableName : true, 
    tableName : '내가 정하는 테이블 이름'
    // sequelize 는 기본적으로 define 함수의 첫 파라미터를 db table 이름으로 사용.
    // 원치 않다면 해당 옵션 true, tableName 정해주기
})
```
