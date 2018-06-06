# MY_Model

## Constructor
public function __construct(&$write_db = null, &$read_db = null)

## CRUD Methods
public function first()

public function find($id)

public function find_by()

public function find_many($values)

public function find_many_by()

public function find_all()

public function insert($data)

- insert_id is more likely for MySQL and not for Oracle, SQL Server, or PostgreSQL. Add solution for SQL Server.

public function insert_batch($data) - **Not working for MSSQL**

public function update($id, $data)

public function update_batch($data, $where_key)

public function update_many($ids, $data)

public function update_by()

public function update_all($data)

public function delete($id)

public function delete_by()

public function delete_many($ids)

public function empty_table($table = NULL)

## Scope Methods

public function soft_delete($val = TRUE)

public function as_array()

public function as_object()

public function as_json()

public function with_deleted()

public function skip_validation($skip = TRUE)

## Utility Methods

public function count_by()

public function count_all()

public function table()

public function format_dropdown()

public function get_field($id = NULL, $field = '')

public function is_unique($field, $value)

## Observers

public function created_on($row)

public function modified_on($row)

## Internal Methods

protected function _return_type($multi = FALSE)

protected function _return_data($data, $multi = FALSE)

protected function _set_where($params, $db_type)

public function trigger($event, $data = false)

public function require_field($field)

public function validate($data, $type = 'update')

public function protect_attributes($row)

protected function set_date($user_date = NULL)

public function get_db_error_message($db_type)

## CI Database Wrappers

public function select($select = '*', $escape = NULL)

public function select_max($select = '', $alias = '')

public function select_min($select = '', $alias = '')

public function select_avg($select = '', $alias = '')

public function select_sum($select = '', $alias = '')

public function distinct($val = TRUE)

public function from($from)

public function join($table, $cond, $type = '')

public function where($key, $value = NULL, $escape = TRUE)

public function or_where($key, $value = NULL, $escape = TRUE)

public function where_in($key = NULL, $values = NULL)

public function or_where_in($key = NULL, $values = NULL)

public function where_not_in($key = NULL, $values = NULL)

public function or_where_not_in($key = NULL, $values = NULL)

public function like($field, $match = '', $side = 'both')

public function not_like($field, $match = '', $side = 'both')

public function or_like($field, $match = '', $side = 'both')

public function or_not_like($field, $match = '', $side = 'both')

public function group_by($by)

public function having($key, $value = '', $escape = TRUE)

public function or_having($key, $value = '', $escape = TRUE)

public function order_by($orderby, $direction = '')

public function limit($value, $offset = '')

public function offset($offset)

public function set($key, $value = '', $escape = TRUE)

public function count_all_results()
