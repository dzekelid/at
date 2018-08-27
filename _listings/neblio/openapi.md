swagger: "2.0"
x-collection-name: Neblio
x-complete: 1
info:
  title: Neblio REST API Suite
  description: apis-for-interacting-with-ntp1-tokens--the-neblio-blockchain
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ins/addr/{address}/utxo:
    get:
      summary: Returns all UTXOs at a given address
      description: Returns information on each Unspent Transaction Output contained
        at an address
      operationId: getAddressUtxos
      x-api-path-slug: insaddraddressutxo-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - ""
      - UTXOs
      - At
      - Given
      - Address
  /testnet/ins/addr/{address}/utxo:
    get:
      summary: Returns all UTXOs at a given address
      description: Returns information on each Unspent Transaction Output contained
        at an address
      operationId: testnet_getAddressUtxos
      x-api-path-slug: testnetinsaddraddressutxo-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - ""
      - UTXOs
      - At
      - Given
      - Address