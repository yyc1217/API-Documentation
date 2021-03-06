# Find Buildings

```
GET /building
```

## Description
> Find buildings of NCU.

# Request
## Headers
<table>
  <tr>
    <td><b>Name</b></td>
    <td><b><b>Required</b></b></td>
    <td><b>Description</b></td>
  </tr>
  <tr>
    <td><b>X-API-NCU-TOKEN</b></td>
    <td><i>yes</i></td>
    <td>Your public API token</td>
  </tr>
</table>

## Example
```
GET /building
```

# Response

## Formats
- json

## Structure
<table>
    <tr>
		<td><b>Filed Name</b></td>
		<td><b>Type</b></td>
		<td><b>Value Description</b></td>
	</tr>
    <tr>
        <td>result</td>
        <td>list</td>
        <td>
			Building Object
            <table>
                <tr>
                    <td>chineseName</td>
                    <td>String</td>
                    <td>building's Chinese name</td>
                </tr>
                <tr>
                    <td>englishName</td>
                    <td>String</td>
                    <td>building's English name</td>
                </tr>
            </table>
        </td>
    </tr>
</table>

## Example
```json
{
	"result" : 
	[
		{
			"chineseName" : "行政大樓",
			"englishName" : "Administrative Building",
		},
		{
			"chineseName" : "總圖書館",
			"englishName" : "Main Library",
		},		
	]
}
```