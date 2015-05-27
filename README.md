# MvcCheckboxList
use of mvc checkboxList with proper alignment,
       <div id="checkbox">
            @{
                
    var htmlListInfo = new MvcCheckBoxList.Model.HtmlListInfo(MvcCheckBoxList.Model.HtmlTag.table, 4, null, MvcCheckBoxList.Model.TextLayout.Default, MvcCheckBoxList.Model.TemplateIsUsed.No);

    if (Model.prj.Count() > 0)
    {       @Html.CheckBoxListFor(model => model.selectedproject,
                                  model => model.prj,
                                  x => x.Id,
                                  x => x.Name,
                                  model => model.userproject,
                                  htmlListInfo)
    }
    else
    {
                <h4>No Project Found</h4>   
    }
            }
        </div>
