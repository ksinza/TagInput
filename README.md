# TagInput
    #setting 
This is a input to select tag  to BlazorServer or Blazor WebAssembly. It is in KsBlazor. KsBlazor  is a  components library to Blazor platform  made by Kevin Sinza 

#how to use?
    #install
    Install-Package KsBlazor -Version 1.0.0 or paket add KsBlazor --version 1.0.0
    
    https://www.nuget.org/packages/KsBlazor/
    
    
    BlazorServer in _Host.cshtml or blazor webassembly in index.html to put the next line in the header:
    
     <link href="_content/KsBlazor/styles.css" rel="stylesheet" />

    
    In the component(yourcomponent.razor) that you want to use  you  must put the next:

    <TagInput Dataset="dataSet"   SelectEvent="selectEvent"></TagInput>
    
    @code{
        public List<DataInputTag> dataSet = new List<DataInputTag>()
        { new DataInputTag(1,"data 1"),
          new DataInputTag(2,"data 2"),
          new DataInputTag(3,"data 3"),
          new DataInputTag(4,"data 4")
        };
    
       void selectEvent(List<DataInputTag> list)
       {

       }
   }

    #customise CSS 
    
