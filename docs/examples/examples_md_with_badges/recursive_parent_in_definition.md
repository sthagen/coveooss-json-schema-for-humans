# Person

- [1. ![Optional](https://img.shields.io/badge/Optional-yellow) Property `Person > relationships`](#relationships)
  - [1.1. ![Optional](https://img.shields.io/badge/Optional-yellow) Property `Person > relationships > mother`](#relationships_mother)
    - [1.1.1. ![Optional](https://img.shields.io/badge/Optional-yellow) Property `Person > relationships > mother > relationships`](#relationships_mother_relationships)
      - [1.1.1.1. ![Optional](https://img.shields.io/badge/Optional-yellow) Property `Person > relationships > mother > relationships > mother`](#relationships_mother_relationships_mother)

**Title:** Person

|                           |                                                                             |
| ------------------------- | --------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                    |
| **Additional properties** | ![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green) |

| Property                           | Pattern | Type   | Deprecated | Definition                                       | Title/Description                            |
| ---------------------------------- | ------- | ------ | ---------- | ------------------------------------------------ | -------------------------------------------- |
| - [relationships](#relationships ) | No      | object | No         | In #/definitions/person/properties/relationships | Relationships between this person and others |

## <a name="relationships"></a>1. ![Optional](https://img.shields.io/badge/Optional-yellow) Property `Person > relationships`

|                           |                                                                             |
| ------------------------- | --------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                    |
| **Additional properties** | ![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green) |
| **Defined in**            | #/definitions/person/properties/relationships                               |

**Description:** Relationships between this person and others

| Property                           | Pattern | Type   | Deprecated | Definition              | Title/Description |
| ---------------------------------- | ------- | ------ | ---------- | ----------------------- | ----------------- |
| - [mother](#relationships_mother ) | No      | object | No         | In #/definitions/person | A human being     |

### <a name="relationships_mother"></a>1.1. ![Optional](https://img.shields.io/badge/Optional-yellow) Property `Person > relationships > mother`

|                           |                                                                             |
| ------------------------- | --------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                    |
| **Additional properties** | ![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green) |
| **Defined in**            | #/definitions/person                                                        |

**Description:** A human being

| Property                                                | Pattern | Type   | Deprecated | Definition | Title/Description                            |
| ------------------------------------------------------- | ------- | ------ | ---------- | ---------- | -------------------------------------------- |
| - [relationships](#relationships_mother_relationships ) | No      | object | No         | -          | Relationships between this person and others |

#### <a name="relationships_mother_relationships"></a>1.1.1. ![Optional](https://img.shields.io/badge/Optional-yellow) Property `Person > relationships > mother > relationships`

|                           |                                                                             |
| ------------------------- | --------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                    |
| **Additional properties** | ![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green) |

**Description:** Relationships between this person and others

| Property                                                | Pattern | Type   | Deprecated | Definition                               | Title/Description |
| ------------------------------------------------------- | ------- | ------ | ---------- | ---------------------------------------- | ----------------- |
| - [mother](#relationships_mother_relationships_mother ) | No      | object | No         | Same as [mother](#relationships_mother ) | A human being     |

##### <a name="relationships_mother_relationships_mother"></a>1.1.1.1. ![Optional](https://img.shields.io/badge/Optional-yellow) Property `Person > relationships > mother > relationships > mother`

|                           |                                                                             |
| ------------------------- | --------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                    |
| **Additional properties** | ![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green) |
| **Same definition as**    | [mother](#relationships_mother)                                             |

**Description:** A human being

----------------------------------------------------------------------------------------------------------------------------
Generated using [json-schema-for-humans](https://github.com/coveooss/json-schema-for-humans)
