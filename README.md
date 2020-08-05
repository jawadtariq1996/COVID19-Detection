# COVID19-Detection
This projects involves experimentation with XRAY dataset to detect COVID19. I used transfer learning and performed different experiments to improve the accuracy of the model. I also used Focal Loss Function to solve the problem of imbalance dataset.

### DataSet Can be Found Here [COVID Datasets2](https://drive.google.com/file/d/1eytbwaLQBv12psV8I-aMkIli9N3bf8nO/view).

### Weights can be Found Here [Model Weights](https://drive.google.com/drive/folders/1WJ6FaGY4FZUmKL7060vW3gQxTVhqeSo8?usp=sharing).


## VGG16 with Binary Cross Entropy

### Training Data

<table>
  <tr><th> COVID19 Class </th><th> Pneumonia Class</th> <th>Normal Class</th> </tr>
<tr><td>

|   Class    | COVID19 | Not COVID19 |
| ---------  |  ----   |  -------    |
| COVID19    |  174    |    26       |
| Not COVID19|   1     |    5999     |

</td><td>

|   Class      | Pneumonia| Not Pneumonia |
| --------     |  -----   |  -------      |
| Pneumonia    |  2023    |    177        |
| Not Pneumonia|   7      |    3993       |
</td><td>

|   Class    | Normal  | Not Normal|
| --------   |  -----  |  -------  |
| Normal     |  3995   |    5      |
| Not Normal |   180   |    2020   |


</td></tr> </table>


### Validation Data
<table>
  <tr><th> COVID19 Class </th><th> Pneumonia Class</th> <th>Normal Class</th> </tr>
<tr><td>

|   Class    | COVID19 | Not COVID19 |
| ---------  |  ----   |  -------    |
| COVID19    |  17     |    11       |
| Not COVID19|   0     |    600      |

</td><td>

|   Class      | Pneumonia| Not Pneumonia |
| --------     |  -----   |  -------      |
| Pneumonia    |  202     |    26         |
| Not Pneumonia|   2      |    398        |
</td><td>

|   Class    | Normal  | Not Normal|
| --------   |  -----  |  -------  |
| Normal     |  399    |    1      |
| Not Normal |   28    |    200    |


</td></tr> </table>


## ResNet18 with Binary Cross Entropy

 ### Training Data
 
<table>
  <tr><th> COVID19 Class </th><th> Pneumonia Class</th> <th>Normal Class</th> </tr>
<tr><td>
  

|   Class    | COVID19 | Not COVID19 |
| ---------  |  ----   |  -------    |
| COVID19    |  188    |    12       |
| Not COVID19|   7     |    5993     |

</td><td>

|   Class      | Pneumonia| Not Pneumonia |
| --------     |  -----   |  -------      |
| Pneumonia    |  1971    |    229        |
| Not Pneumonia|   7      |    3993       |
</td><td>

|   Class    | Normal  | Not Normal|
| --------   |  -----  |  -------  |
| Normal     |  3993   |    7      |
| Not Normal |   221   |    1979   |

</td></tr> </table>

### Validation Data

<table>
  <tr><th> COVID19 Class </th><th> Pneumonia Class</th> <th>Normal Class</th> </tr>
<tr><td>
  

|   Class    | COVID19 | Not COVID19 |
| ---------  |  ----   |  -------    |
| COVID19    |  22     |    6        |
| Not COVID19|   4     |    596      |

</td><td>

|   Class      | Pneumonia| Not Pneumonia |
| --------     |  -----   |  -------      |
| Pneumonia    |  213     |    15         |
| Not Pneumonia|   9      |    391        |
</td><td>

|   Class    | Normal  | Not Normal|
| --------   |  -----  |  -------  |
| Normal     |  391    |    9      |
| Not Normal |  15     |    213    |

</td></tr> </table>


## VGG16 with Focal Loss

 ### Training Data
 
<table>
  <tr><th> COVID19 Class </th><th> Pneumonia Class</th> <th>Normal Class</th> </tr>
<tr><td>
  

|   Class    | COVID19 | Not COVID19 |
| ---------  |  ----   |  -------    |
| COVID19    |  190    |    10       |
| Not COVID19|   8     |    5992     |

</td><td>

|   Class      | Pneumonia| Not Pneumonia |
| --------     |  -----   |  -------      |
| Pneumonia    |  2133    |    67         |
| Not Pneumonia|   80     |    3920       |
</td><td>

|   Class    | Normal  | Not Normal|
| --------   |  -----  |  -------  |
| Normal     |  3913   |    87     |
| Not Normal |   61    |    2139   |

</td></tr> </table>

### Validation Data

<table>
  <tr><th> COVID19 Class </th><th> Pneumonia Class</th> <th>Normal Class</th> </tr>
<tr><td>
  

|   Class    | COVID19 | Not COVID19 |
| ---------  |  ----   |  -------    |
| COVID19    |  23     |    5        |
| Not COVID19|   0     |    600      |

</td><td>

|   Class      | Pneumonia| Not Pneumonia |
| --------     |  -----   |  -------      |
| Pneumonia    |  212     |    16         |
| Not Pneumonia|   10     |    390        |
</td><td>

|   Class    | Normal  | Not Normal|
| --------   |  -----  |  -------  |
| Normal     |  391    |    9      |
| Not Normal |  16     |    212    |

</td></tr> </table>

## ResNet18 with Focal Loss

 ### Training Data
 
<table>
  <tr><th> COVID19 Class </th><th> Pneumonia Class</th> <th>Normal Class</th> </tr>
<tr><td>
  

|   Class    | COVID19 | Not COVID19 |
| ---------  |  ----   |  -------    |
| COVID19    |  192    |    8        |
| Not COVID19|   55    |    5945     |

</td><td>

|   Class      | Pneumonia| Not Pneumonia |
| --------     |  -----   |  -------      |
| Pneumonia    |  2119    |    81         |
| Not Pneumonia|   242    |    3758       |
</td><td>

|   Class    | Normal  | Not Normal|
| --------   |  -----  |  -------  |
| Normal     |  3760   |    240    |
| Not Normal |   87    |    2113   |

</td></tr> </table>

### Validation Data

<table>
  <tr><th> COVID19 Class </th><th> Pneumonia Class</th> <th>Normal Class</th> </tr>
<tr><td>
  

|   Class    | COVID19 | Not COVID19 |
| ---------  |  ----   |  -------    |
| COVID19    |  25     |    3        |
| Not COVID19|   4     |    596      |

</td><td>

|   Class      | Pneumonia| Not Pneumonia |
| --------     |  -----   |  -------      |
| Pneumonia    |  215     |    13         |
| Not Pneumonia|   29     |    371        |
</td><td>

|   Class    | Normal  | Not Normal|
| --------   |  -----  |  -------  |
| Normal     |  368    |    32     |
| Not Normal |  13     |    215    |

</td></tr> </table>



## Experiments Details:

|   Model         |     Loss Functions      |  Focal Loss Parms |  F1 Score: COVID19 | 
| --------------  |     -----------------   | ----------------- | -----------------  |      
|   VGG16         |        BCE              |                   |     0.81           |
|   ResNet18      |        BCE              |                   |     0.76           |     
|   VGG16         |        Focal Loss       |     a =2, g =2    |     0.90           |      
|   ResNet18      |        Focal Los        |     a1 = 1 g=2    |     0.88           |  

