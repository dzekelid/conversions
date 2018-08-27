swagger: "2.0"
x-collection-name: Trello
x-complete: 1
info:
  title: Trello
  description: this-document-describes-the-rest-api-of-trello-as-published-by-trello-com---a-hrefhttpstrello-comdocsindex-html-target-blankofficial-documentationa--a-hrefhttpstrello-comdocsapi-target-blankthe-html-pages-that-were-scraped-in-order-to-generate-this-specification-a
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cards/{idCard}/checklist/{idChecklist}/checkItem/{idCheckItem}/convertToCard:
    post:
      summary: Post Cards Checklist Checkitem Checkitem Converttocard
      description: Post cards checklist checkitem checkitem converttocard.
      operationId: addCardsChecklistCheckItemConvertToCardByIdCardByIdChecklistByIdCheckItem
      x-api-path-slug: cardsidcardchecklistidchecklistcheckitemidcheckitemconverttocard-post
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idCheckItem
        description: idCheckItem
      - in: path
        name: idChecklist
        description: idChecklist
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Checklist
      - Checkitem
      - Checkitem
      - Converttocard