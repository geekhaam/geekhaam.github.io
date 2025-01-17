---
layout: post
title: "JSP: Day07 - Session"
comment: true
categories: JSP Session
---
# 세션(Session)

- 세션도 쿠키와 마찬가지로 서버와의 관계를 유지하기 위한 수단입니다.
- 단, 쿠키와 달리 클라이언트의 특정 위치에 저장되는 것이 아니라, **서버 상에 객체 형태**로 존재합니다.
- 서버당 하나의 세션 객체를 가질 수 있습니다.
- 세션 객체는 브라우저 창을 종료하면 삭제됩니다.
- 따라서 세션은 서버에서만 접근이 가능하여 보안이 좋고, 저장할 수 있는 데이터에 한계가 없습니다.
- 세션은 클라이언트의 요청이 발생하면 자동생성되어 고유한 ID값을 클라이언트에 넘겨주며 이것은 쿠키에 저장됩니다.
- JSP에서는 session이라는 내장 객체를 지원하여 세션의 속성을 설정할 수 있습니다.

* **session 객체 관련 메서드**

    1. `setAttribute()` - 세션에 데이터를 저장합니다.
    2. `getAttribute()` - 세션에 저장되어 있는 데이터를 얻습니다.
    3. `getAttributeNames()` - 세션에 저장되어 있는 모든 데이터의 세션 이름(key)을 얻습니다.
    4. `getId()` - 자동생성된 세션의 유니크한 아이디를 얻습니다.
    5. `getCreationTime()` - 세션이 생성된 시간을 구합니다.
    6. `getLastAccessedTime()` - 웹 브라우저가 가장 마지막에 세션에 접근한 시간을 구합니다.
    7. `setMaxInactiveInterval()` - 세션의 유효시간을 설정합니다. 초 단위로 기록합니다.
    8. `getMaxInactiveInterval()` - 세션의 유효시간을 얻습니다. 가장 최근 요청시점을 기준으로 카운트됩니다.
    9. `removeAttribute()` - 특정 세션을 삭제합니다.
    10. `invalidate()` - 모든 세션을 삭제합니다.