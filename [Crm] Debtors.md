Manage debtor data like addresses and other contact data.

## cURL


## Laravel Api
### show()
This function uses strict by database strucutred data.   
By giving the correct Debtor unique identifier the function returns all debtor data back. 

**Show**  
```php
use Mainpixel\Api\Types\Crm\Debtors;  

public function show($id,Debtors $debtors){  
    $debtorData = $debtors->show(['identifier' => $id]);  
    return view('...',$debtorData);
}
```
| Variable      | Function      |
| ------------- |:-------------:|
| identifier    | Unique debtorID  |

> You can get an unique identifier by using the list option.
