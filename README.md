# TagInput
This is a input to select tag  to BlazorServer or Blazor WebAssembly 

how to use?


    <TagInput Dataset="dataSet"   SelectEvent="selectEvent"></TagInput>
    
    public List<DataInputTag> dataSet = new List<DataInputTag>()
    { new DataInputTag(1,"data 1"),
      new DataInputTag(2,"data 2"),
      new DataInputTag(3,"data 3"),
      new DataInputTag(4,"data 4")
    };
    
     void selectEvent(List<DataInputTag> list)
    {

    }
