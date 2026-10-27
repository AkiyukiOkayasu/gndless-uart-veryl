# Changelog

## [Unreleased]

### Added

- framing errorとfalse startからの復帰を検証するtestを追加した

### Changed

- `CLK_FREQ / BAUD_RATE >= 2`と`DATA_WIDTH >= 1`のパラメータ契約をdoc commentへ明記した

## [0.1.1] - 2026-08-08

- 公開moduleのparam/port doc commentを追加し、説明文の途中改行を整理
- doc commentの句点と体言止めの表記を整理
- doc commentのsummary表記を統一
- UART受信testのdoc commentへ検証対象を明記
- `UartRx`の`clk_cnt`/`bit_cnt`をparameter導出の必要最小幅へ変更

## [0.1.0] - 2026-07-31

### Changed

- UART receiverを独立packageへ移動
- `UartRx`へLSB-first frame、中央sampling、`valid`のWavedromを追加
