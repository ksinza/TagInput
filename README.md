# TagInput
    #setting 
This is a input to select tag  to BlazorServer or Blazor WebAssembly. It is in KsBlazor. KsBlazor  is a  components library to Blazor platform  made by Kevin Sinza 

#how to use?
    
    install
    
    Install-Package KsBlazor -Version 1.0.0 or paket add KsBlazor --version 1.0.0
    
    https://www.nuget.org/packages/KsBlazor/
    
    
    BlazorServer in _Host.cshtml or blazor webassembly in index.html to put the next line in the header:
    
     <link href="_content/KsBlazor/styles.css" rel="stylesheet" />

    
    In the component(yourcomponent.razor) that you want to use  you  must put the next:
    
    @using KsBlazor.TagInput
    
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
        the next style already it is done in library,  this is to show you   the  class rules   and you can edit how you wish it.
        
        style default
        
            .mainSelect {
                position: relative;
                height: auto;
                width: 100%;
                display: inline-grid;
            }

            #menu {
                border-radius: 7px;
                height: auto;
                border-color: black;
                width: 100%;
                border: 1px solid;
                margin-top: 0%;
                position: relative;
                border-top-right-radius: 0;
                border-top-left-radius: 0;
            }

            #select {
                margin-bottom: 0%;
                height: 20%;
                width: 70%;
                margin-bottom: 0%;
                width: 100%;
                display: block;
            }

            .values {
                position: absolute;
                width: 100%;
                width: -moz-available; /* WebKit-based browsers will ignore this. */
                width: -webkit-fill-available; /* Mozilla-based browsers will ignore this. */
                width: fill-available;
                height: auto;
                top: 0;
            }

            .selectData {
                display: inline-flex;
                background: #e4f2f9;
                border-radius: 8px;
                border: 1px solid;
                width: auto;
                padding-left: 1%;
                padding-right: 0.4%;
                margin-top: 0.7%;
                font-weight: bold;
                color: black;
                width: 24%;
            }

            .closeSelect {
              
                cursor: pointer;
                font-size: 0.7rem;
                float: right;
                color: black;
                font-weight: bold;
            }

            #menu li {
                cursor: pointer;
                list-style: none;
                margin: 3px;
                padding-left: 1px;
            }

                #menu li p {
                    display: inline-block;
                    width: 13px;
                    margin-right: 7px;
                    height: 2px;
                }

            #menu ul {
                padding: 0;
            }

            .itemSelect {
                padding-right: 7px;
                margin: 0px;
                height: 21px;
                width: 90%;
                white-space: nowrap;
                overflow: hidden;
                text-overflow: ellipsis;
                font-size: 1rem;
            }
            }

            .countselect {
                display: inline-flex;
            }

            .search {
                padding-left: 23px !important;
            }
