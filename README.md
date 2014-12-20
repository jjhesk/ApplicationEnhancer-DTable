ApplicationEnhancer-DTable
=================

Enhanced Application interface from using DTable from https://datatables.net/examples/


### Configuration
key | explaination 
--- | --- 
table_id | the table id without #
table_implementation | the full implementation object json from [https://datatables.net/examples/basic_init/multi_col_sort.html]
_domain | default with the current domain on the URL bar
_interaction |  default will support click tap and touch

### Example
```javascript


var table_app = new DApp({
    table_id: "my_table",
    table_implementation: {
        processing: true,
        "order": [ 1, 'desc' ],
        ajax: "",
        columns: [
            { data: "transid"},
            { data: "time"},
            { data: "count"},
            { data: "ref_code"}
        ],
        "dom": '<"back_to_reg_log"><"feature_button"><"datepicker">lfrtip',
        "initComplete": null
    }

});
```
