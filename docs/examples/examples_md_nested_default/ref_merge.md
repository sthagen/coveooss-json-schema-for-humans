# Test

- [1. [Optional] Property Test > aProperty](#aProperty)
- [2. [Optional] Property Test > aDictPropertyARequired](#aDictPropertyARequired)
  - [2.1. [Required] Property Test > aDictPropertyARequired > a](#aDictPropertyARequired_a)
  - [2.2. [Required] Property Test > aDictPropertyARequired > b](#aDictPropertyARequired_b)

**Title:** Test

|                           |                  |
| ------------------------- | ---------------- |
| **Type**                  | `object`         |
| **Required**              | No               |
| **Additional properties** | Any type allowed |

<details>
<summary>
<strong> <a name="aProperty"></a>1. [Optional] Property Test > aProperty</strong>  

</summary>
<blockquote>

**Title:** Title from definition

|                |                           |
| -------------- | ------------------------- |
| **Type**       | `enum (of string)`        |
| **Required**   | No                        |
| **Default**    | `"Default from property"` |
| **Defined in** | #/definitions/aProperty   |

**Description:** This is the description from the definition

Must be one of:
* "value1"
* "value2"

</blockquote>
</details>

<details>
<summary>
<strong> <a name="aDictPropertyARequired"></a>2. [Optional] Property Test > aDictPropertyARequired</strong>  

</summary>
<blockquote>

|                           |                             |
| ------------------------- | --------------------------- |
| **Type**                  | `object`                    |
| **Required**              | No                          |
| **Additional properties** | Any type allowed            |
| **Default**               | `{"a": "a", "b": "b"}`      |
| **Defined in**            | #/definitions/aDictProperty |

<details>
<summary>
<strong> <a name="aDictPropertyARequired_a"></a>2.1. [Required] Property Test > aDictPropertyARequired > a</strong>  

</summary>
<blockquote>

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | Yes      |

</blockquote>
</details>

<details>
<summary>
<strong> <a name="aDictPropertyARequired_b"></a>2.2. [Required] Property Test > aDictPropertyARequired > b</strong>  

</summary>
<blockquote>

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | Yes      |

</blockquote>
</details>

</blockquote>
</details>

----------------------------------------------------------------------------------------------------------------------------
Generated using [json-schema-for-humans](https://github.com/coveooss/json-schema-for-humans)